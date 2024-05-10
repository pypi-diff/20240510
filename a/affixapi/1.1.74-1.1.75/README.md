# Comparing `tmp/affixapi-1.1.74.tar.gz` & `tmp/affixapi-1.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.74.tar", last modified: Fri May 10 12:46:44 2024, max compression
+gzip compressed data, was "affixapi-1.1.75.tar", last modified: Fri May 10 13:50:49 2024, max compression
```

## Comparing `affixapi-1.1.74.tar` & `affixapi-1.1.75.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 12:46:36.000000 affixapi-1.1.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 12:46:44.441792 affixapi-1.1.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-10 12:46:36.000000 affixapi-1.1.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.417791 affixapi-1.1.74/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.421792 affixapi-1.1.74/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.421792 affixapi-1.1.74/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.429792 affixapi-1.1.74/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17888 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24681 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.429792 affixapi-1.1.74/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 12:46:44.441792 affixapi-1.1.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 12:46:36.000000 affixapi-1.1.74/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.032359 affixapi-1.1.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 13:50:45.000000 affixapi-1.1.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 13:50:49.032359 affixapi-1.1.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-10 13:50:45.000000 affixapi-1.1.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.032359 affixapi-1.1.75/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 13:50:48.000000 affixapi-1.1.75/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 13:50:49.000000 affixapi-1.1.75/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:50:48.000000 affixapi-1.1.75/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 13:50:48.000000 affixapi-1.1.75/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:50:48.000000 affixapi-1.1.75/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.008359 affixapi-1.1.75/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.008359 affixapi-1.1.75/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.008359 affixapi-1.1.75/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.020359 affixapi-1.1.75/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24681 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17375 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17403 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.020359 affixapi-1.1.75/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-10 13:50:45.000000 affixapi-1.1.75/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 13:50:49.032359 affixapi-1.1.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 13:50:45.000000 affixapi-1.1.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:50:49.032359 affixapi-1.1.75/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-10 13:50:45.000000 affixapi-1.1.75/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.74/LICENSE` & `affixapi-1.1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/PKG-INFO` & `affixapi-1.1.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.74
+Version: 1.1.75
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `affixapi-1.1.74/README.md` & `affixapi-1.1.75/README.md`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.75/affixapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.74
+Version: 1.1.75
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `affixapi-1.1.74/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.75/affixapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/__init__.py` & `affixapi-1.1.75/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.75/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/api/core_api.py` & `affixapi-1.1.75/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/api/management_api.py` & `affixapi-1.1.75/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.75/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/api_client.py` & `affixapi-1.1.75/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/apis/__init__.py` & `affixapi-1.1.75/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/configuration.py` & `affixapi-1.1.75/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/exceptions.py` & `affixapi-1.1.75/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.75/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/address_response.py` & `affixapi-1.1.75/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/client_request.py` & `affixapi-1.1.75/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/client_response.py` & `affixapi-1.1.75/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.75/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/company_response.py` & `affixapi-1.1.75/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/compensation_history_no_non_null_request.py` & `affixapi-1.1.75/openapi_client/model/compensation_history_no_non_null_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,52 +94,55 @@
         return {
             'pay_rate': (float,),  # noqa: E501
             'pay_period': (str,),  # noqa: E501
             'pay_frequency': (str,),  # noqa: E501
             'employment_type': (str,),  # noqa: E501
             'currency': (CurrencyNotNullRequest,),  # noqa: E501
             'effective_date': (date,),  # noqa: E501
+            'notes': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'pay_rate': 'pay_rate',  # noqa: E501
         'pay_period': 'pay_period',  # noqa: E501
         'pay_frequency': 'pay_frequency',  # noqa: E501
         'employment_type': 'employment_type',  # noqa: E501
         'currency': 'currency',  # noqa: E501
         'effective_date': 'effective_date',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
+    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, notes, *args, **kwargs):  # noqa: E501
         """CompensationHistoryNoNonNullRequest - a model defined in OpenAPI
 
         Args:
             pay_rate (float):
             pay_period (str):
             pay_frequency (str):
             employment_type (str):
             currency (CurrencyNotNullRequest):
             effective_date (date):
+            notes (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -195,14 +198,15 @@
 
         self.pay_rate = pay_rate
         self.pay_period = pay_period
         self.pay_frequency = pay_frequency
         self.employment_type = employment_type
         self.currency = currency
         self.effective_date = effective_date
+        self.notes = notes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/compensation_history_response.py` & `affixapi-1.1.75/openapi_client/model/compensation_history_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,52 +98,55 @@
         return {
             'pay_rate': (float, none_type,),  # noqa: E501
             'pay_period': (str, none_type,),  # noqa: E501
             'pay_frequency': (str, none_type,),  # noqa: E501
             'employment_type': (str, none_type,),  # noqa: E501
             'currency': (CurrencyResponse,),  # noqa: E501
             'effective_date': (date, none_type,),  # noqa: E501
+            'notes': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'pay_rate': 'pay_rate',  # noqa: E501
         'pay_period': 'pay_period',  # noqa: E501
         'pay_frequency': 'pay_frequency',  # noqa: E501
         'employment_type': 'employment_type',  # noqa: E501
         'currency': 'currency',  # noqa: E501
         'effective_date': 'effective_date',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
+    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, notes, *args, **kwargs):  # noqa: E501
         """CompensationHistoryResponse - a model defined in OpenAPI
 
         Args:
             pay_rate (float, none_type):
             pay_period (str, none_type):
             pay_frequency (str, none_type):
             employment_type (str, none_type):
             currency (CurrencyResponse):
             effective_date (date, none_type):
+            notes (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -199,14 +202,15 @@
 
         self.pay_rate = pay_rate
         self.pay_period = pay_period
         self.pay_frequency = pay_frequency
         self.employment_type = employment_type
         self.currency = currency
         self.effective_date = effective_date
+        self.notes = notes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/create_employee_request.py` & `affixapi-1.1.75/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.75/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.75/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.75/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.75/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.75/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/currency_response.py` & `affixapi-1.1.75/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/disconnect_response.py` & `affixapi-1.1.75/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employee_response.py` & `affixapi-1.1.75/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.75/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.75/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employment_history_no_non_null_request.py` & `affixapi-1.1.75/openapi_client/model/employment_history_no_non_null_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,50 +74,56 @@
         """
         return {
             'job_title': (str,),  # noqa: E501
             'effective_date': (date,),  # noqa: E501
             'group_id': (str, none_type,),  # noqa: E501
             'group_remote_id': (str, none_type,),  # noqa: E501
             'group_name': (str, none_type,),  # noqa: E501
+            'manager_id': (str, none_type,),  # noqa: E501
+            'manager_remote_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'job_title': 'job_title',  # noqa: E501
         'effective_date': 'effective_date',  # noqa: E501
         'group_id': 'group_id',  # noqa: E501
         'group_remote_id': 'group_remote_id',  # noqa: E501
         'group_name': 'group_name',  # noqa: E501
+        'manager_id': 'manager_id',  # noqa: E501
+        'manager_remote_id': 'manager_remote_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_title, effective_date, group_id, group_remote_id, group_name, *args, **kwargs):  # noqa: E501
+    def __init__(self, job_title, effective_date, group_id, group_remote_id, group_name, manager_id, manager_remote_id, *args, **kwargs):  # noqa: E501
         """EmploymentHistoryNoNonNullRequest - a model defined in OpenAPI
 
         Args:
             job_title (str):
             effective_date (date):
             group_id (str, none_type):
             group_remote_id (str, none_type):
             group_name (str, none_type):
+            manager_id (str, none_type):
+            manager_remote_id (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -172,14 +178,16 @@
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.job_title = job_title
         self.effective_date = effective_date
         self.group_id = group_id
         self.group_remote_id = group_remote_id
         self.group_name = group_name
+        self.manager_id = manager_id
+        self.manager_remote_id = manager_remote_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/employment_history_response.py` & `affixapi-1.1.75/openapi_client/model/location_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.address_response import AddressResponse
+    globals()['AddressResponse'] = AddressResponse
 
-class EmploymentHistoryResponse(ModelNormal):
+
+class LocationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,68 +60,69 @@
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'job_title': (str, none_type,),  # noqa: E501
-            'effective_date': (date, none_type,),  # noqa: E501
-            'group_id': (str, none_type,),  # noqa: E501
-            'group_remote_id': (str, none_type,),  # noqa: E501
-            'group_name': (str, none_type,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'remote_id': (str, none_type,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
+            'address': (AddressResponse,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'job_title': 'job_title',  # noqa: E501
-        'effective_date': 'effective_date',  # noqa: E501
-        'group_id': 'group_id',  # noqa: E501
-        'group_remote_id': 'group_remote_id',  # noqa: E501
-        'group_name': 'group_name',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'remote_id': 'remote_id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'address': 'address',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_title, effective_date, group_id, group_remote_id, group_name, *args, **kwargs):  # noqa: E501
-        """EmploymentHistoryResponse - a model defined in OpenAPI
+    def __init__(self, id, remote_id, name, type, address, *args, **kwargs):  # noqa: E501
+        """LocationResponse - a model defined in OpenAPI
 
         Args:
-            job_title (str, none_type):
-            effective_date (date, none_type):
-            group_id (str, none_type):
-            group_remote_id (str, none_type):
-            group_name (str, none_type):
+            id (str, none_type): The Affix-assigned id of the individual
+            remote_id (str, none_type): the remote system-assigned id of the individual
+            name (str, none_type): System assigned description of the location
+            type (str, none_type): The location's type. In cases where there is no clear mapping, the original value passed through will be returned. 
+            address (AddressResponse):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -167,19 +172,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.job_title = job_title
-        self.effective_date = effective_date
-        self.group_id = group_id
-        self.group_remote_id = group_remote_id
-        self.group_name = group_name
+        self.id = id
+        self.remote_id = remote_id
+        self.name = name
+        self.type = type
+        self.address = address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/employment_status_not_null_not_nullable.py` & `affixapi-1.1.75/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.75/openapi_client/model/employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/employment_status_response.py` & `affixapi-1.1.75/openapi_client/model/employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.75/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/group_response.py` & `affixapi-1.1.75/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.75/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.75/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.75/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/identity_response.py` & `affixapi-1.1.75/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/inline_response400.py` & `affixapi-1.1.75/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/inline_response401.py` & `affixapi-1.1.75/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/inline_response409.py` & `affixapi-1.1.75/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/introspect_response.py` & `affixapi-1.1.75/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.75/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/location_response.py` & `affixapi-1.1.75/openapi_client/model/payslip_response_contributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,16 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
-def lazy_import():
-    from openapi_client.model.address_response import AddressResponse
-    globals()['AddressResponse'] = AddressResponse
 
-
-class LocationResponse(ModelNormal):
+class PayslipResponseContributions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,69 +56,59 @@
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (str, none_type,),  # noqa: E501
-            'remote_id': (str, none_type,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
-            'type': (str, none_type,),  # noqa: E501
-            'address': (AddressResponse,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'amount': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'remote_id': 'remote_id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'address': 'address',  # noqa: E501
+        'amount': 'amount',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, name, type, address, *args, **kwargs):  # noqa: E501
-        """LocationResponse - a model defined in OpenAPI
+    def __init__(self, name, amount, *args, **kwargs):  # noqa: E501
+        """PayslipResponseContributions - a model defined in OpenAPI
 
         Args:
-            id (str, none_type): The Affix-assigned id of the individual
-            remote_id (str, none_type): the remote system-assigned id of the individual
-            name (str, none_type): System assigned description of the location
-            type (str, none_type): The location's type. In cases where there is no clear mapping, the original value passed through will be returned. 
-            address (AddressResponse):
+            name (str):
+            amount (float): if USD/EUR/GBP, in cent
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -172,19 +158,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.remote_id = remote_id
         self.name = name
-        self.type = type
-        self.address = address
+        self.amount = amount
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/message_response.py` & `affixapi-1.1.75/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/mode_request.py` & `affixapi-1.1.75/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/mode_response.py` & `affixapi-1.1.75/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/payrun_response.py` & `affixapi-1.1.75/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.75/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/payslip_response.py` & `affixapi-1.1.75/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.75/openapi_client/model/payslip_response_deductions.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PayslipResponseContributions(ModelNormal):
+class PayslipResponseDeductions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -96,15 +96,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, name, amount, *args, **kwargs):  # noqa: E501
-        """PayslipResponseContributions - a model defined in OpenAPI
+        """PayslipResponseDeductions - a model defined in OpenAPI
 
         Args:
             name (str):
             amount (float): if USD/EUR/GBP, in cent
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `affixapi-1.1.74/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.75/openapi_client/model/payslip_response_earnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PayslipResponseDeductions(ModelNormal):
+class PayslipResponseEarnings(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,44 +71,47 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
             'amount': (float,),  # noqa: E501
+            'hours': (float, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'amount': 'amount',  # noqa: E501
+        'hours': 'hours',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, amount, *args, **kwargs):  # noqa: E501
-        """PayslipResponseDeductions - a model defined in OpenAPI
+    def __init__(self, name, amount, hours, *args, **kwargs):  # noqa: E501
+        """PayslipResponseEarnings - a model defined in OpenAPI
 
         Args:
             name (str):
             amount (float): if USD/EUR/GBP, in cent
+            hours (float, none_type): hours, if applicable
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -160,14 +163,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.amount = amount
+        self.hours = hours
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.75/openapi_client/model/payslip_response_taxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PayslipResponseEarnings(ModelNormal):
+class PayslipResponseTaxes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,47 +71,47 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
             'amount': (float,),  # noqa: E501
-            'hours': (float, none_type,),  # noqa: E501
+            'employer_tax': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'amount': 'amount',  # noqa: E501
-        'hours': 'hours',  # noqa: E501
+        'employer_tax': 'employer_tax',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, amount, hours, *args, **kwargs):  # noqa: E501
-        """PayslipResponseEarnings - a model defined in OpenAPI
+    def __init__(self, name, amount, employer_tax, *args, **kwargs):  # noqa: E501
+        """PayslipResponseTaxes - a model defined in OpenAPI
 
         Args:
             name (str):
             amount (float): if USD/EUR/GBP, in cent
-            hours (float, none_type): hours, if applicable
+            employer_tax (bool, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -163,15 +163,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.amount = amount
-        self.hours = hours
+        self.employer_tax = employer_tax
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.74/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.75/openapi_client/model/policy_type_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,96 +24,98 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PayslipResponseTaxes(ModelNormal):
+class PolicyTypeResponse(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('value',): {
+            'None': None,
+            'NULL': "null",
+            'BEREAVEMENT': "bereavement",
+            'HOLIDAY': "holiday",
+            'JURY_DUTY': "jury_duty",
+            'PERSONAL': "personal",
+            'SICK': "sick",
+            'VACATION': "vacation",
+            'VOLUNTEER': "volunteer",
+        },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
-            'amount': (float,),  # noqa: E501
-            'employer_tax': (bool, none_type,),  # noqa: E501
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'amount': 'amount',  # noqa: E501
-        'employer_tax': 'employer_tax',  # noqa: E501
-    }
+    attribute_map = {}
 
-    _composed_schemas = {}
+    _composed_schemas = None
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, amount, employer_tax, *args, **kwargs):  # noqa: E501
-        """PayslipResponseTaxes - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """PolicyTypeResponse - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            name (str):
-            amount (float): if USD/EUR/GBP, in cent
-            employer_tax (bool, none_type):
+            args[0] (str):, must be one of ["null", "bereavement", "holiday", "jury_duty", "personal", "sick", "vacation", "volunteer", ]  # noqa: E501
 
         Keyword Args:
+            value (str):, must be one of ["null", "bereavement", "holiday", "jury_duty", "personal", "sick", "vacation", "volunteer", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -137,18 +139,31 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -160,19 +175,17 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
-        self.amount = amount
-        self.employer_tax = employer_tax
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
```

### Comparing `affixapi-1.1.74/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.75/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/policy_type_response.py` & `affixapi-1.1.75/openapi_client/model/tokens_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PolicyTypeResponse(ModelSimple):
+class TokensResponse(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -45,46 +45,35 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'None': None,
-            'NULL': "null",
-            'BEREAVEMENT': "bereavement",
-            'HOLIDAY': "holiday",
-            'JURY_DUTY': "jury_duty",
-            'PERSONAL': "personal",
-            'SICK': "sick",
-            'VACATION': "vacation",
-            'VOLUNTEER': "volunteer",
-        },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'value': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -99,23 +88,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """PolicyTypeResponse - a model defined in OpenAPI
+        """TokensResponse - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["null", "bereavement", "holiday", "jury_duty", "personal", "sick", "vacation", "volunteer", ]  # noqa: E501
+            args[0] ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]):  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["null", "bereavement", "holiday", "jury_duty", "personal", "sick", "vacation", "volunteer", ]  # noqa: E501
+            value ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]):  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.74/openapi_client/model/provider_request.py` & `affixapi-1.1.75/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/provider_response.py` & `affixapi-1.1.75/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/providers_response.py` & `affixapi-1.1.75/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/scopes_request.py` & `affixapi-1.1.75/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/scopes_response.py` & `affixapi-1.1.75/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.75/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.75/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.75/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.75/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/timesheet_response.py` & `affixapi-1.1.75/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.75/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/token_request.py` & `affixapi-1.1.75/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/token_response.py` & `affixapi-1.1.75/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/model/tokens_response.py` & `affixapi-1.1.75/openapi_client/model/work_locations20230301_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.location_response import LocationResponse
+    globals()['LocationResponse'] = LocationResponse
 
-class TokensResponse(ModelSimple):
+
+class WorkLocations20230301Response(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -64,16 +68,17 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
+            'value': ([LocationResponse],),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -88,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TokensResponse - a model defined in OpenAPI
+        """WorkLocations20230301Response - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]):  # noqa: E501
+            args[0] ([LocationResponse]): Work locations.  # noqa: E501
 
         Keyword Args:
-            value ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]):  # noqa: E501
+            value ([LocationResponse]): Work locations.  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.74/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.75/openapi_client/model/employment_history_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,30 +23,30 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
-def lazy_import():
-    from openapi_client.model.location_response import LocationResponse
-    globals()['LocationResponse'] = LocationResponse
 
-
-class WorkLocations20230301Response(ModelSimple):
+class EmploymentHistoryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
@@ -68,48 +68,64 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'value': ([LocationResponse],),
+            'job_title': (str, none_type,),  # noqa: E501
+            'effective_date': (date, none_type,),  # noqa: E501
+            'group_id': (str, none_type,),  # noqa: E501
+            'group_remote_id': (str, none_type,),  # noqa: E501
+            'group_name': (str, none_type,),  # noqa: E501
+            'manager_id': (str, none_type,),  # noqa: E501
+            'manager_remote_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
+    attribute_map = {
+        'job_title': 'job_title',  # noqa: E501
+        'effective_date': 'effective_date',  # noqa: E501
+        'group_id': 'group_id',  # noqa: E501
+        'group_remote_id': 'group_remote_id',  # noqa: E501
+        'group_name': 'group_name',  # noqa: E501
+        'manager_id': 'manager_id',  # noqa: E501
+        'manager_remote_id': 'manager_remote_id',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """WorkLocations20230301Response - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def __init__(self, job_title, effective_date, group_id, group_remote_id, group_name, manager_id, manager_remote_id, *args, **kwargs):  # noqa: E501
+        """EmploymentHistoryResponse - a model defined in OpenAPI
 
         Args:
-            args[0] ([LocationResponse]): Work locations.  # noqa: E501
+            job_title (str, none_type):
+            effective_date (date, none_type):
+            group_id (str, none_type):
+            group_remote_id (str, none_type):
+            group_name (str, none_type):
+            manager_id (str, none_type):
+            manager_remote_id (str, none_type):
 
         Keyword Args:
-            value ([LocationResponse]): Work locations.  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -133,31 +149,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -169,17 +172,23 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
+
+        self.job_title = job_title
+        self.effective_date = effective_date
+        self.group_id = group_id
+        self.group_remote_id = group_remote_id
+        self.group_name = group_name
+        self.manager_id = manager_id
+        self.manager_remote_id = manager_remote_id
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
```

### Comparing `affixapi-1.1.74/openapi_client/model_utils.py` & `affixapi-1.1.75/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/models/__init__.py` & `affixapi-1.1.75/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/openapi_client/rest.py` & `affixapi-1.1.75/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/setup.py` & `affixapi-1.1.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.74"
+VERSION = "1.1.75"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.74/test/test_2023_03_01_api.py` & `affixapi-1.1.75/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_address_no_non_null_request.py` & `affixapi-1.1.75/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_address_response.py` & `affixapi-1.1.75/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_client_request.py` & `affixapi-1.1.75/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_client_response.py` & `affixapi-1.1.75/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_companies20230301_response.py` & `affixapi-1.1.75/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_company_response.py` & `affixapi-1.1.75/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_compensation_history_no_non_null_request.py` & `affixapi-1.1.75/test/test_compensation_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_compensation_history_response.py` & `affixapi-1.1.75/test/test_compensation_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_core_api.py` & `affixapi-1.1.75/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_create_employee_request.py` & `affixapi-1.1.75/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.75/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_create_employee_request_dependents.py` & `affixapi-1.1.75/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.75/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_create_employee_request_manager.py` & `affixapi-1.1.75/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_currency_not_null_request.py` & `affixapi-1.1.75/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_currency_response.py` & `affixapi-1.1.75/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_disconnect_response.py` & `affixapi-1.1.75/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employee_response.py` & `affixapi-1.1.75/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employee_response_manager.py` & `affixapi-1.1.75/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employees20230301_response.py` & `affixapi-1.1.75/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employment_history_no_non_null_request.py` & `affixapi-1.1.75/test/test_employment_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employment_history_response.py` & `affixapi-1.1.75/test/test_employment_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employment_status_not_null_not_nullable.py` & `affixapi-1.1.75/test/test_employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employment_status_not_null_request.py` & `affixapi-1.1.75/test/test_employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_employment_status_response.py` & `affixapi-1.1.75/test/test_employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_group_no_null_enum_request.py` & `affixapi-1.1.75/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_group_response.py` & `affixapi-1.1.75/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_groups20230301_response.py` & `affixapi-1.1.75/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.75/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_id_and_message_response.py` & `affixapi-1.1.75/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_identity_response.py` & `affixapi-1.1.75/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_inline_response400.py` & `affixapi-1.1.75/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_inline_response401.py` & `affixapi-1.1.75/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_inline_response409.py` & `affixapi-1.1.75/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_introspect_response.py` & `affixapi-1.1.75/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_location_no_non_null_request.py` & `affixapi-1.1.75/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_location_response.py` & `affixapi-1.1.75/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_management_api.py` & `affixapi-1.1.75/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_message_response.py` & `affixapi-1.1.75/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_mode_request.py` & `affixapi-1.1.75/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_mode_response.py` & `affixapi-1.1.75/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payrun_response.py` & `affixapi-1.1.75/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payruns20230301_response.py` & `affixapi-1.1.75/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslip_response.py` & `affixapi-1.1.75/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslip_response_contributions.py` & `affixapi-1.1.75/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslip_response_deductions.py` & `affixapi-1.1.75/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslip_response_earnings.py` & `affixapi-1.1.75/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslip_response_taxes.py` & `affixapi-1.1.75/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_payslips20230301_response.py` & `affixapi-1.1.75/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_policy_type_response.py` & `affixapi-1.1.75/test/test_policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_provider_request.py` & `affixapi-1.1.75/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_provider_response.py` & `affixapi-1.1.75/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_providers_response.py` & `affixapi-1.1.75/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_scopes_request.py` & `affixapi-1.1.75/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_scopes_response.py` & `affixapi-1.1.75/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_time_off_balance_response.py` & `affixapi-1.1.75/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.75/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.75/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_time_off_entry_response.py` & `affixapi-1.1.75/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_timesheet_response.py` & `affixapi-1.1.75/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_timesheets20230301_response.py` & `affixapi-1.1.75/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_token_request.py` & `affixapi-1.1.75/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_token_response.py` & `affixapi-1.1.75/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_tokens_response.py` & `affixapi-1.1.75/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_work_locations20230301_response.py` & `affixapi-1.1.75/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.74/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.75/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

