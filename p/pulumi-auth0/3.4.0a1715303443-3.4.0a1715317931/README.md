# Comparing `tmp/pulumi_auth0-3.4.0a1715303443.tar.gz` & `tmp/pulumi_auth0-3.4.0a1715317931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_auth0-3.4.0a1715303443.tar", last modified: Fri May 10 01:20:39 2024, max compression
+gzip compressed data, was "pulumi_auth0-3.4.0a1715317931.tar", last modified: Fri May 10 05:14:47 2024, max compression
```

## Comparing `pulumi_auth0-3.4.0a1715303443.tar` & `pulumi_auth0-3.4.0a1715317931.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.751930 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   363124 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)   104781 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    70116 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    31095 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_signing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    31241 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    21295 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_members.py
--rw-r--r--   0 runner    (1001) docker     (127)   528303 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_custom_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_partials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35493 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    50702 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54738 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   363124 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104781 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70116 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/custom_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/email_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31095 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/email_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_signing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31241 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21295 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)   528303 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt_custom_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt_partials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35493 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/rule_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50702 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/trigger_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54738 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 05:14:47.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-10 05:14:47.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:14:47.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 05:14:47.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 05:14:47.000000 pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-10 05:14:41.000000 pulumi_auth0-3.4.0a1715317931/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:14:47.715887 pulumi_auth0-3.4.0a1715317931/setup.cfg
```

### Comparing `pulumi_auth0-3.4.0a1715303443/PKG-INFO` & `pulumi_auth0-3.4.0a1715317931/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1715303443
+Version: 3.4.0a1715317931
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1715303443/README.md` & `pulumi_auth0-3.4.0a1715317931/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/__init__.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_inputs.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_utilities.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/action.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/attack_protection.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding_theme.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_credentials.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_grant.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/client_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.pyi` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/vars.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_client.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_clients.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/connection_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain_verification.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/custom_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_provider.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/email_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_template.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/email_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_attack_protection.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding_theme.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_client.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_connection.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_custom_domain.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_organization.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_pages.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_resource_server.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_role.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_signing_keys.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_signing_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_tenant.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_user.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/guardian.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/guardian.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/hook.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/log_stream.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connection.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connections.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_role.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_roles.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_member_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_members.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/organization_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/outputs.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pages.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_custom_text.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt_custom_text.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_partials.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/prompt_partials.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/provider.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scope.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scopes.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/resource_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permission.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permissions.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/role_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule_config.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/rule_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/tenant.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_action.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/trigger_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_actions.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permission.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permissions.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_role.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_roles.py` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/PKG-INFO` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1715303443
+Version: 3.4.0a1715317931
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/SOURCES.txt` & `pulumi_auth0-3.4.0a1715317931/pulumi_auth0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

