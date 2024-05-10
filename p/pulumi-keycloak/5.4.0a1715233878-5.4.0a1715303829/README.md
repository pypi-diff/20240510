# Comparing `tmp/pulumi_keycloak-5.4.0a1715233878.tar.gz` & `tmp/pulumi_keycloak-5.4.0a1715303829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.4.0a1715233878.tar", last modified: Thu May  9 05:56:35 2024, max compression
+gzip compressed data, was "pulumi_keycloak-5.4.0a1715303829.tar", last modified: Fri May 10 01:28:41 2024, max compression
```

## Comparing `pulumi_keycloak-5.4.0a1715233878.tar` & `pulumi_keycloak-5.4.0a1715303829.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.510097 pulumi_keycloak-5.4.0a1715233878/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-09 05:56:35.510097 pulumi_keycloak-5.4.0a1715233878/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.494097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87704 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22086 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.498097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24528 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16759 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23258 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.498097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23101 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    27392 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.498097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/custom_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19227 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    44994 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    89182 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.498097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70026 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    82372 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.506097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28807 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22842 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31347 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26324 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31089 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35208 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36162 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31190 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    34346 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30627 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    79430 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    25176 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.510097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    63709 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)   100920 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28397 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20291 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:56:35.510097 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-09 05:56:35.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-09 05:56:35.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:56:35.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 05:56:35.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 05:56:35.000000 pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 05:56:29.000000 pulumi_keycloak-5.4.0a1715233878/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:56:35.510097 pulumi_keycloak-5.4.0a1715233878/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.486349 pulumi_keycloak-5.4.0a1715303829/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-10 01:28:41.486349 pulumi_keycloak-5.4.0a1715303829/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.470349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87704 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22086 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.474349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24528 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16759 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23258 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.474349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23101 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27392 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.478349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/custom_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19227 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44994 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89182 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.478349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70026 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82372 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.486349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28807 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22842 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31347 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26324 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31089 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35208 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36162 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31190 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34346 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30627 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79430 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25176 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.486349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63709 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100920 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28397 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20291 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:28:41.486349 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-10 01:28:41.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-10 01:28:41.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:28:41.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:28:41.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 01:28:41.000000 pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-10 01:28:35.000000 pulumi_keycloak-5.4.0a1715303829/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:28:41.490349 pulumi_keycloak-5.4.0a1715303829/setup.cfg
```

### Comparing `pulumi_keycloak-5.4.0a1715233878/PKG-INFO` & `pulumi_keycloak-5.4.0a1715303829/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1715233878
+Version: 5.4.0a1715303829
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1715233878/README.md` & `pulumi_keycloak-5.4.0a1715303829/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/bindings.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/execution_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/authentication/subflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/__init__.pyi` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/custom_user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/default_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/generic_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_authentication_execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_authentication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_client_description_converter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/get_user_realm_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/group_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/custom_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/custom_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/ldap/user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/oidc/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/realm_user_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/required_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/role.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client_default_scope.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client_default_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/get_client_installation_provider.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/get_client_installation_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1715233878
+Version: 5.4.0a1715303829
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1715233878/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.4.0a1715303829/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1715233878/pyproject.toml` & `pulumi_keycloak-5.4.0a1715303829/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_keycloak"
   description = "A Pulumi package for creating and managing keycloak cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "keycloak"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.4.0a1715233878"
+  version = "5.4.0a1715303829"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-keycloak"
 
 [build-system]
```

