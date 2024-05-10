# Comparing `tmp/pulumi_ise-0.2.0a1715349279.tar.gz` & `tmp/pulumi_ise-0.2.0a1715356962.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ise-0.2.0a1715349279.tar", last modified: Fri May 10 14:01:47 2024, max compression
+gzip compressed data, was "pulumi_ise-0.2.0a1715356962.tar", last modified: Fri May 10 16:05:02 2024, max compression
```

## Comparing `pulumi_ise-0.2.0a1715349279.tar` & `pulumi_ise-0.2.0a1715356962.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.083759 pulumi_ise-0.2.0a1715349279/pulumi_ise/
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.087759 pulumi_ise-0.2.0a1715349279/pulumi_ise/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.091759 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80156 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/allowed_protocols_tacacs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50601 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authentication_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    45277 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    43476 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_global_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    44897 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    28863 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_allowed_protocols_tacacs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authentication_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_global_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_policy_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_tacacs_command_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_tacacs_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_time_and_date_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)   116498 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44443 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/policy_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/tacacs_command_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/tacacs_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32331 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/time_and_date_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.095759 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_add_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_join_domain_with_all_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    75887 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_join_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    26681 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/certificate_authentication_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    55166 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/endpoint_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_active_directory_groups_by_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_active_directory_join_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_certificate_authentication_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_endpoint_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_identity_source_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_internal_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_user_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/identity_source_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    34526 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/internal_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/user_identity_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.095759 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   112154 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/device_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/get_device_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/network/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.099759 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    82293 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   211450 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/allowed_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    50615 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authentication_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    44600 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    42799 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_global_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    75898 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    44220 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    28923 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/downloadable_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    58584 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_allowed_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authentication_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_global_exception_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22064 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_downloadable_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_policy_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_time_and_date_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)   120674 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44461 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/policy_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    32345 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/time_and_date_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/get_license_tier_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/license_tier_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18240 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/system/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/egress_matrix_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_egress_matrix_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_ip_to_sgt_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_ip_to_sgt_mapping_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_security_group_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    19913 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/ip_to_sgt_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/ip_to_sgt_mapping_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13741 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13964 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/security_group_acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-10 14:01:47.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-10 14:01:47.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:01:47.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 14:01:47.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 14:01:47.000000 pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 14:01:40.000000 pulumi_ise-0.2.0a1715349279/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:01:47.103759 pulumi_ise-0.2.0a1715349279/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.678068 pulumi_ise-0.2.0a1715356962/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-10 16:05:02.678068 pulumi_ise-0.2.0a1715356962/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.658068 pulumi_ise-0.2.0a1715356962/pulumi_ise/
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.658068 pulumi_ise-0.2.0a1715356962/pulumi_ise/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.662068 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80156 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/allowed_protocols_tacacs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50601 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authentication_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45277 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43476 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_global_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44897 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28863 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_allowed_protocols_tacacs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authentication_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_global_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_policy_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_tacacs_command_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_tacacs_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_time_and_date_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116498 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44443 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/policy_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/tacacs_command_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/tacacs_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32331 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/time_and_date_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.666068 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_add_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_join_domain_with_all_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75887 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_join_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26681 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/certificate_authentication_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55166 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/endpoint_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_active_directory_groups_by_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_active_directory_join_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_certificate_authentication_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_endpoint_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_identity_source_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_internal_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_user_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/identity_source_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34526 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/internal_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/user_identity_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.670068 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112154 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/device_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/get_device_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/network/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.674068 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82293 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211450 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/allowed_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50615 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authentication_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44600 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42799 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_global_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75898 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44220 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28923 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/downloadable_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58584 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_allowed_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authentication_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_global_exception_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22064 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_downloadable_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_policy_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_time_and_date_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120674 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44461 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/policy_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32345 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/time_and_date_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.674068 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/get_license_tier_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/license_tier_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18240 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/system/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.678068 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/egress_matrix_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_egress_matrix_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_ip_to_sgt_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_ip_to_sgt_mapping_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_security_group_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19913 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/ip_to_sgt_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/ip_to_sgt_mapping_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13741 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13964 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/security_group_acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:05:02.678068 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-10 16:05:02.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-10 16:05:02.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:05:02.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 16:05:02.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 16:05:02.000000 pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 16:04:56.000000 pulumi_ise-0.2.0a1715356962/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:05:02.678068 pulumi_ise-0.2.0a1715356962/setup.cfg
```

### Comparing `pulumi_ise-0.2.0a1715349279/PKG-INFO` & `pulumi_ise-0.2.0a1715356962/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ise
-Version: 0.2.0a1715349279
+Version: 0.2.0a1715356962
 Summary: A Pulumi package for managing resources on a Cisco ISE (Identity Service Engine) instance.
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-ise
 Project-URL: Repository, https://github.com/pulumi/pulumi-ise
 Keywords: pulumi,ise,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ise-0.2.0a1715349279/README.md` & `pulumi_ise-0.2.0a1715356962/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/__init__.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/_utilities.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/config/__init__.pyi` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/config/vars.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/__init__.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/_inputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/allowed_protocols_tacacs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/allowed_protocols_tacacs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authentication_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authentication_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_global_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_global_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/authorization_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/authorization_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_allowed_protocols_tacacs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_allowed_protocols_tacacs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authentication_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authentication_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_global_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_global_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_authorization_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_authorization_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_policy_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_policy_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_tacacs_command_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_tacacs_command_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_tacacs_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_tacacs_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/get_time_and_date_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/get_time_and_date_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/outputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/policy_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/policy_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/tacacs_command_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/tacacs_command_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/tacacs_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/tacacs_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/deviceadmin/time_and_date_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/deviceadmin/time_and_date_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/__init__.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/_inputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_add_groups.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_add_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_join_domain_with_all_nodes.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_join_domain_with_all_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/active_directory_join_point.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/active_directory_join_point.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/certificate_authentication_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/certificate_authentication_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/endpoint.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/endpoint_identity_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/endpoint_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_active_directory_groups_by_domain.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_active_directory_groups_by_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_active_directory_join_point.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_active_directory_join_point.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_certificate_authentication_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_certificate_authentication_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_endpoint.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_endpoint_identity_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_endpoint_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_identity_source_sequence.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_identity_source_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_internal_user.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_internal_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/get_user_identity_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/get_user_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/identity_source_sequence.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/identity_source_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/internal_user.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/internal_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/outputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/identitymanagement/user_identity_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/identitymanagement/user_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/_inputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/device.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/device_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/device_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/get_device.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/get_device_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/get_device_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/network/outputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/__init__.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/_inputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/allowed_protocols.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/allowed_protocols.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authentication_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authentication_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_global_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_global_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/authorization_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/authorization_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/dictionary.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/dictionary.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/downloadable_acl.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/downloadable_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_allowed_protocols.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_allowed_protocols.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authentication_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authentication_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_global_exception_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_global_exception_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_profile.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_authorization_rule.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_authorization_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_dictionary.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_dictionary.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_downloadable_acl.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_downloadable_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_policy_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_policy_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/get_time_and_date_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/get_time_and_date_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/outputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/policy_set.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/policy_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/networkaccess/time_and_date_condition.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/networkaccess/time_and_date_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/provider.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/_inputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/get_license_tier_state.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/get_license_tier_state.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/get_repository.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/license_tier_state.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/license_tier_state.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/outputs.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/system/repository.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/system/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/__init__.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/egress_matrix_cell.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/egress_matrix_cell.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_egress_matrix_cell.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_egress_matrix_cell.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_ip_to_sgt_mapping.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_ip_to_sgt_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_ip_to_sgt_mapping_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_ip_to_sgt_mapping_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_security_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/get_security_group_acl.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/get_security_group_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/ip_to_sgt_mapping.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/ip_to_sgt_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/ip_to_sgt_mapping_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/ip_to_sgt_mapping_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/security_group.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise/trustsec/security_group_acl.py` & `pulumi_ise-0.2.0a1715356962/pulumi_ise/trustsec/security_group_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/PKG-INFO` & `pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ise
-Version: 0.2.0a1715349279
+Version: 0.2.0a1715356962
 Summary: A Pulumi package for managing resources on a Cisco ISE (Identity Service Engine) instance.
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-ise
 Project-URL: Repository, https://github.com/pulumi/pulumi-ise
 Keywords: pulumi,ise,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ise-0.2.0a1715349279/pulumi_ise.egg-info/SOURCES.txt` & `pulumi_ise-0.2.0a1715356962/pulumi_ise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ise-0.2.0a1715349279/pyproject.toml` & `pulumi_ise-0.2.0a1715356962/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ise"
   description = "A Pulumi package for managing resources on a Cisco ISE (Identity Service Engine) instance."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ise", "category/network"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.2.0a1715349279"
+  version = "0.2.0a1715356962"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://github.com/pulumi/pulumi-ise"
     Repository = "https://github.com/pulumi/pulumi-ise"
 
 [build-system]
```

