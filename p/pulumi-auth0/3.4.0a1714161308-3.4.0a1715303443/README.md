# Comparing `tmp/pulumi_auth0-3.4.0a1714161308.tar.gz` & `tmp/pulumi_auth0-3.4.0a1715303443.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_auth0-3.4.0a1714161308.tar", last modified: Fri Apr 26 19:57:33 2024, max compression
+gzip compressed data, was "pulumi_auth0-3.4.0a1715303443.tar", last modified: Fri May 10 01:20:39 2024, max compression
```

## Comparing `pulumi_auth0-3.4.0a1714161308.tar` & `pulumi_auth0-3.4.0a1715303443.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:33.668016 pulumi_auth0-3.4.0a1714161308/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-26 19:57:33.668016 pulumi_auth0-3.4.0a1714161308/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:33.664016 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   363124 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/branding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)   104781 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:33.668016 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    70116 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/custom_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/email_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    31095 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/email_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_branding_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_signing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    31241 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    21295 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_members.py
--rw-r--r--   0 runner    (1001) docker     (127)   528303 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt_custom_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt_partials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35493 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/rule_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    50702 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/trigger_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54738 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:33.668016 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-26 19:57:33.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-26 19:57:33.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:57:33.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 19:57:33.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 19:57:33.000000 pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-26 19:57:27.000000 pulumi_auth0-3.4.0a1714161308/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:57:33.668016 pulumi_auth0-3.4.0a1714161308/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.751930 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   363124 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104781 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70116 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31095 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_signing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31241 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21295 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)   528303 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_custom_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_partials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35493 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50702 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54738 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 01:20:39.000000 pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-10 01:20:31.000000 pulumi_auth0-3.4.0a1715303443/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:20:39.755931 pulumi_auth0-3.4.0a1715303443/setup.cfg
```

### Comparing `pulumi_auth0-3.4.0a1714161308/PKG-INFO` & `pulumi_auth0-3.4.0a1715303443/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1714161308
+Version: 3.4.0a1715303443
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1714161308/README.md` & `pulumi_auth0-3.4.0a1715303443/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/__init__.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/_inputs.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/_utilities.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/action.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/attack_protection.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/branding.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/branding_theme.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client_credentials.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_credentials.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,18 +20,14 @@
                  client_id: pulumi.Input[str],
                  client_secret: Optional[pulumi.Input[str]] = None,
                  private_key_jwt: Optional[pulumi.Input['ClientCredentialsPrivateKeyJwtArgs']] = None):
         """
         The set of arguments for constructing a ClientCredentials resource.
         :param pulumi.Input[str] authentication_method: Configure the method to use when making requests to any endpoint that requires this client to authenticate. Options include `none` (public client without a client secret), `client_secret_post` (confidential client using HTTP POST parameters), `client_secret_basic` (confidential client using HTTP Basic), `private_key_jwt` (confidential client using a Private Key JWT).
         :param pulumi.Input[str] client_id: The ID of the client for which to configure the authentication method.
-        :param pulumi.Input[str] client_secret: Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-               To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-               will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-               authentication method.
         :param pulumi.Input['ClientCredentialsPrivateKeyJwtArgs'] private_key_jwt: Defines `private_key_jwt` client authentication method.
         """
         pulumi.set(__self__, "authentication_method", authentication_method)
         pulumi.set(__self__, "client_id", client_id)
         if client_secret is not None:
             pulumi.set(__self__, "client_secret", client_secret)
         if private_key_jwt is not None:
@@ -60,20 +56,14 @@
     @client_id.setter
     def client_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter(name="clientSecret")
     def client_secret(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-        To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-        will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-        authentication method.
-        """
         return pulumi.get(self, "client_secret")
 
     @client_secret.setter
     def client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_secret", value)
 
     @property
@@ -96,18 +86,14 @@
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
                  private_key_jwt: Optional[pulumi.Input['ClientCredentialsPrivateKeyJwtArgs']] = None):
         """
         Input properties used for looking up and filtering ClientCredentials resources.
         :param pulumi.Input[str] authentication_method: Configure the method to use when making requests to any endpoint that requires this client to authenticate. Options include `none` (public client without a client secret), `client_secret_post` (confidential client using HTTP POST parameters), `client_secret_basic` (confidential client using HTTP Basic), `private_key_jwt` (confidential client using a Private Key JWT).
         :param pulumi.Input[str] client_id: The ID of the client for which to configure the authentication method.
-        :param pulumi.Input[str] client_secret: Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-               To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-               will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-               authentication method.
         :param pulumi.Input['ClientCredentialsPrivateKeyJwtArgs'] private_key_jwt: Defines `private_key_jwt` client authentication method.
         """
         if authentication_method is not None:
             pulumi.set(__self__, "authentication_method", authentication_method)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if client_secret is not None:
@@ -138,20 +124,14 @@
     @client_id.setter
     def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter(name="clientSecret")
     def client_secret(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-        To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-        will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-        authentication method.
-        """
         return pulumi.get(self, "client_secret")
 
     @client_secret.setter
     def client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_secret", value)
 
     @property
@@ -199,18 +179,14 @@
 
         This is to be expected, because the pem file can't be checked for differences.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] authentication_method: Configure the method to use when making requests to any endpoint that requires this client to authenticate. Options include `none` (public client without a client secret), `client_secret_post` (confidential client using HTTP POST parameters), `client_secret_basic` (confidential client using HTTP Basic), `private_key_jwt` (confidential client using a Private Key JWT).
         :param pulumi.Input[str] client_id: The ID of the client for which to configure the authentication method.
-        :param pulumi.Input[str] client_secret: Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-               To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-               will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-               authentication method.
         :param pulumi.Input[pulumi.InputType['ClientCredentialsPrivateKeyJwtArgs']] private_key_jwt: Defines `private_key_jwt` client authentication method.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ClientCredentialsArgs,
@@ -294,18 +270,14 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] authentication_method: Configure the method to use when making requests to any endpoint that requires this client to authenticate. Options include `none` (public client without a client secret), `client_secret_post` (confidential client using HTTP POST parameters), `client_secret_basic` (confidential client using HTTP Basic), `private_key_jwt` (confidential client using a Private Key JWT).
         :param pulumi.Input[str] client_id: The ID of the client for which to configure the authentication method.
-        :param pulumi.Input[str] client_secret: Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-               To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-               will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-               authentication method.
         :param pulumi.Input[pulumi.InputType['ClientCredentialsPrivateKeyJwtArgs']] private_key_jwt: Defines `private_key_jwt` client authentication method.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClientCredentialsState.__new__(_ClientCredentialsState)
 
         __props__.__dict__["authentication_method"] = authentication_method
@@ -329,20 +301,14 @@
         The ID of the client for which to configure the authentication method.
         """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter(name="clientSecret")
     def client_secret(self) -> pulumi.Output[str]:
-        """
-        Secret for the client when using `client_secret_post` or `client_secret_basic` authentication method. Keep this private.
-        To access this attribute you need to add the `read:client_keys` scope to the Terraform client. Otherwise, the attribute
-        will contain an empty string. The attribute will also be an empty string in case `private_key_jwt` is selected as an
-        authentication method.
-        """
         return pulumi.get(self, "client_secret")
 
     @property
     @pulumi.getter(name="privateKeyJwt")
     def private_key_jwt(self) -> pulumi.Output[Optional['outputs.ClientCredentialsPrivateKeyJwt']]:
         """
         Defines `private_key_jwt` client authentication method.
```

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/client_grant.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/client_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/__init__.pyi` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/config/vars.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection_client.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/connection_clients.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/connection_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/custom_domain.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/custom_domain_verification.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/custom_domain_verification.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,33 +38,27 @@
 class _CustomDomainVerificationState:
     def __init__(__self__, *,
                  cname_api_key: Optional[pulumi.Input[str]] = None,
                  custom_domain_id: Optional[pulumi.Input[str]] = None,
                  origin_domain_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering CustomDomainVerification resources.
-        :param pulumi.Input[str] cname_api_key: The value of the `cname-api-key` header to send when forwarding requests. Only present if the type of the custom domain
-               is `self_managed_certs` and Terraform originally managed the domain's verification.
         :param pulumi.Input[str] custom_domain_id: ID of the custom domain resource.
         :param pulumi.Input[str] origin_domain_name: The DNS name of the Auth0 origin server that handles traffic for the custom domain.
         """
         if cname_api_key is not None:
             pulumi.set(__self__, "cname_api_key", cname_api_key)
         if custom_domain_id is not None:
             pulumi.set(__self__, "custom_domain_id", custom_domain_id)
         if origin_domain_name is not None:
             pulumi.set(__self__, "origin_domain_name", origin_domain_name)
 
     @property
     @pulumi.getter(name="cnameApiKey")
     def cname_api_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The value of the `cname-api-key` header to send when forwarding requests. Only present if the type of the custom domain
-        is `self_managed_certs` and Terraform originally managed the domain's verification.
-        """
         return pulumi.get(self, "cname_api_key")
 
     @cname_api_key.setter
     def cname_api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cname_api_key", value)
 
     @property
@@ -187,16 +181,14 @@
         """
         Get an existing CustomDomainVerification resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cname_api_key: The value of the `cname-api-key` header to send when forwarding requests. Only present if the type of the custom domain
-               is `self_managed_certs` and Terraform originally managed the domain's verification.
         :param pulumi.Input[str] custom_domain_id: ID of the custom domain resource.
         :param pulumi.Input[str] origin_domain_name: The DNS name of the Auth0 origin server that handles traffic for the custom domain.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CustomDomainVerificationState.__new__(_CustomDomainVerificationState)
 
@@ -204,18 +196,14 @@
         __props__.__dict__["custom_domain_id"] = custom_domain_id
         __props__.__dict__["origin_domain_name"] = origin_domain_name
         return CustomDomainVerification(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="cnameApiKey")
     def cname_api_key(self) -> pulumi.Output[str]:
-        """
-        The value of the `cname-api-key` header to send when forwarding requests. Only present if the type of the custom domain
-        is `self_managed_certs` and Terraform originally managed the domain's verification.
-        """
         return pulumi.get(self, "cname_api_key")
 
     @property
     @pulumi.getter(name="customDomainId")
     def custom_domain_id(self) -> pulumi.Output[str]:
         """
         ID of the custom domain resource.
```

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/email_provider.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/email_template.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/email_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_attack_protection.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_branding.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_branding_theme.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_branding_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_client.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_connection.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_custom_domain.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_organization.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_pages.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_resource_server.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_role.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_signing_keys.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_signing_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_tenant.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/get_user.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/guardian.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/guardian.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/hook.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/log_stream.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_connection.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_connections.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member_role.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_member_roles.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_member_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/organization_members.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/organization_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/outputs.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/pages.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt_custom_text.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_custom_text.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/prompt_partials.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/prompt_partials.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/provider.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server_scope.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/resource_server_scopes.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/resource_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role_permission.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/role_permissions.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/role_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/rule.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/rule_config.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/rule_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/tenant.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/trigger_action.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/trigger_actions.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_permission.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_permissions.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_role.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0/user_roles.py` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/PKG-INFO` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 3.4.0a1714161308
+Version: 3.4.0a1715303443
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Keywords: pulumi,auth0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_auth0-3.4.0a1714161308/pulumi_auth0.egg-info/SOURCES.txt` & `pulumi_auth0-3.4.0a1715303443/pulumi_auth0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-3.4.0a1714161308/pyproject.toml` & `pulumi_auth0-3.4.0a1715303443/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_auth0"
   description = "A Pulumi package for creating and managing auth0 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "auth0"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1714161308"
+  version = "3.4.0a1715303443"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-auth0"
 
 [build-system]
```

