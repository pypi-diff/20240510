# Comparing `tmp/pulumi_vault-6.2.0a1715230012.tar.gz` & `tmp/pulumi_vault-6.2.0a1715237402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vault-6.2.0a1715230012.tar", last modified: Thu May  9 04:51:28 2024, max compression
+gzip compressed data, was "pulumi_vault-6.2.0a1715237402.tar", last modified: Thu May  9 06:53:54 2024, max compression
```

## Comparing `pulumi_vault-6.2.0a1715230012.tar` & `pulumi_vault-6.2.0a1715237402.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.702475 pulumi_vault-6.2.0a1715230012/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-09 04:51:28.702475 pulumi_vault-6.2.0a1715230012/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.658475 pulumi_vault-6.2.0a1715230012/pulumi_vault/
--rw-r--r--   0 runner    (1001) docker     (127)    31033 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72858 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.662474 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    92141 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    23726 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.662474 pulumi_vault-6.2.0a1715230012/pulumi_vault/alicloud/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/alicloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/alicloud/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.662474 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23349 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    46431 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    31784 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_role_secret_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/get_auth_backend_role_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/audit_request_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/auth_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.666475 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    32638 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23132 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_config_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_identity_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)   100480 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_roletag_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_sts_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/get_static_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    49429 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    48158 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.666475 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    54712 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    29094 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    39016 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    72069 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/cert_auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.666475 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/ui_custom_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.666475 pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39516 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    41519 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.670475 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   290762 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   253519 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73181 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    36862 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30781 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_static_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    98074 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secrets_mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/egp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.670475 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    51908 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24796 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_impersonated_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_roleset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27271 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_static_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.674475 pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39069 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_nomad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/get_raft_autopilot_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.674475 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56415 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/github/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.678475 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_client_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_openid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    37454 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17298 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_member_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_member_group_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20235 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    23627 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_login_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    23768 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    29427 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29733 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_key_allowed_client_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21920 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.678475 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66052 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.682475 pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37775 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    54405 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14770 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.682475 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31174 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    47419 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_service_account_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    50716 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    55709 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.682475 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret_subkeys_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secrets_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secrets_list_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    18979 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret_backend_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.686475 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84686 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/get_dynamic_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/get_static_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    77475 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_dynamic_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_library_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    23975 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.686475 pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29276 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    25164 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28237 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25344 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_totp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.686475 pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    40909 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    42018 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/nomad_secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/nomad_secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.690475 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38338 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    16937 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/password_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.694475 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/backend_config_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49695 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_crl_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    61789 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    36625 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)   116221 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    68833 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_root_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    58420 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)    48576 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/quota_lease_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    25625 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/quota_rate_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.694475 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34622 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    21858 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30059 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/raft_autopilot.py
--rw-r--r--   0 runner    (1001) docker     (127)    74915 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/raft_snapshot_agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/rgp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.694475 pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    46027 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.694475 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17911 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    38565 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_aws_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    32274 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_azure_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26233 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_gcp_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    32177 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_gh_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_github_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    26648 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_vercel_destination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.698475 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17875 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/secret_backend_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    72399 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.698475 pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26293 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    43363 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.698475 pulumi_vault-6.2.0a1715230012/pulumi_vault/tokenauth/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/tokenauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52075 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/tokenauth/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.698475 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/get_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/get_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25599 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.698475 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/get_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/get_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)    53286 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/secret_cache_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:28.702475 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-09 04:51:28.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-09 04:51:28.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:51:28.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:51:28.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 04:51:28.000000 pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 04:51:22.000000 pulumi_vault-6.2.0a1715230012/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:51:28.702475 pulumi_vault-6.2.0a1715230012/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.139299 pulumi_vault-6.2.0a1715237402/pulumi_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)    31033 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72858 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.139299 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92141 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23726 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.139299 pulumi_vault-6.2.0a1715237402/pulumi_vault/alicloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/alicloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/alicloud/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.143300 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23349 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46431 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31784 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_role_secret_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/get_auth_backend_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/audit_request_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/auth_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.143300 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32638 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23132 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_config_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_identity_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100480 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_roletag_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_sts_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/get_static_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49429 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48158 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.147300 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54712 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29094 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39016 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72069 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/cert_auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.147300 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/ui_custom_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.147300 pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39516 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41519 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.151300 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   290762 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253519 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73181 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36862 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30781 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_static_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98074 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secrets_mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/egp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.151300 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51908 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24796 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_impersonated_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_roleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27271 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_static_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.151300 pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39069 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_nomad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/get_raft_autopilot_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.151300 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56415 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/github/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.159300 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_client_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_openid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37454 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17298 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_member_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_member_group_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20235 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23627 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_login_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23768 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29427 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29733 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_key_allowed_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21920 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.159300 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66052 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.159300 pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37775 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54405 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14770 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.159300 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31174 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47419 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_service_account_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50716 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55709 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.163300 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret_subkeys_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secrets_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secrets_list_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18979 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret_backend_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.163300 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84686 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/get_dynamic_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/get_static_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77475 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_dynamic_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_library_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23975 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.167300 pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29276 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25164 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28237 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25344 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_totp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.167300 pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40909 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42018 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/nomad_secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/nomad_secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.167300 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38338 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16937 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/password_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.171300 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/backend_config_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49695 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_crl_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61789 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36625 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116221 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68833 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_root_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58420 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48576 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/quota_lease_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25625 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/quota_rate_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.171300 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34622 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21858 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30059 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/raft_autopilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74915 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/raft_snapshot_agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/rgp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.171300 pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46027 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.175300 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17911 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38565 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_aws_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32274 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_azure_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26233 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_gcp_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32177 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_gh_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_github_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26648 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_vercel_destination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.175300 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17875 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/secret_backend_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72399 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.175300 pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26293 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43363 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.175300 pulumi_vault-6.2.0a1715237402/pulumi_vault/tokenauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/tokenauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52075 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/tokenauth/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/get_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/get_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25599 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/get_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/get_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53286 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/secret_cache_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-09 06:53:54.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-09 06:53:54.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:53:54.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:53:54.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 06:53:54.000000 pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 06:53:47.000000 pulumi_vault-6.2.0a1715237402/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:53:54.179300 pulumi_vault-6.2.0a1715237402/setup.cfg
```

### Comparing `pulumi_vault-6.2.0a1715230012/PKG-INFO` & `pulumi_vault-6.2.0a1715237402/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.2.0a1715230012
+Version: 6.2.0a1715237402
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.2.0a1715230012/README.md` & `pulumi_vault-6.2.0a1715237402/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/_utilities.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/get_access_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_library.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ad/secret_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ad/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/alicloud/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/alicloud/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_login.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/auth_backend_role_secret_id.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/auth_backend_role_secret_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/approle/get_auth_backend_role_id.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/approle/get_auth_backend_role_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/audit.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/audit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/audit_request_header.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/audit_request_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_cert.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_client.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_config_identity.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_config_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_identity_whitelist.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_identity_whitelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_login.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_role_tag.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_roletag_blacklist.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_roletag_blacklist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/auth_backend_sts_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/auth_backend_sts_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/get_access_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/get_static_access_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/get_static_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/aws/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/aws/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/auth_backend_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/get_access_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/azure/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/cert_auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/cert_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/config/__init__.pyi` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/config/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/config/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/config/ui_custom_message.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/config/ui_custom_message.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/config/vars.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/consul/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/consul/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_connection.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/database/secrets_mount.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/database/secrets_mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/egp_policy.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/egp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/get_auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_impersonated_account.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_impersonated_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_roleset.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_roleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/gcp/secret_static_account.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/gcp/secret_static_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/endpoint.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/get_secret.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/generic/secret.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/generic/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_auth_backends.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_auth_backends.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_namespace.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_namespaces.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_nomad_access_token.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_nomad_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_policy_document.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_policy_document.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/get_raft_autopilot_state.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/get_raft_autopilot_state.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/github/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/github/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/github/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/github/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/github/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/github/team.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/github/user.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/github/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity_alias.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/entity_policies.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/entity_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_entity.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_group.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_client_creds.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_client_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_openid_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_openid_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/get_oidc_public_keys.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/get_oidc_public_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_alias.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_member_entity_ids.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_member_entity_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_member_group_ids.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_member_group_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/group_policies.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_duo.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_login_enforcement.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_login_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_okta.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_pingid.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/mfa_totp.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_assignment.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_client.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_key.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_key_allowed_client_id.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_key_allowed_client_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_provider.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/oidc_scope.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/oidc_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/identity/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/identity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/jwt/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/jwt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kmip/secret_scope.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kmip/secret_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/auth_backend_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_auth_backend_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/get_service_account_token.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/get_service_account_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kubernetes/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kubernetes/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret_subkeys_v2.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret_subkeys_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secret_v2.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secrets_list.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secrets_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/get_secrets_list_v2.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/get_secrets_list_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret_backend_v2.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret_backend_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/kv/secret_v2.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/kv/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend_group.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/auth_backend_user.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/get_dynamic_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/get_dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/get_static_credentials.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/get_static_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_dynamic_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_dynamic_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_library_set.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_library_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ldap/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ldap/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/keys.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/managed/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/managed/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_duo.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_okta.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_pingid.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mfa_totp.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mongodbatlas/secret_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mongodbatlas/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/mount.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/namespace.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/nomad_secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/nomad_secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/nomad_secret_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/nomad_secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend_group.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/auth_backend_user.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/okta/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/password_policy.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/password_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/backend_config_cluster.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/backend_config_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_issuer.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_issuer.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_issuers.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_key.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/get_backend_keys.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/get_backend_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_cert.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_ca.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_issuers.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_config_urls.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_config_urls.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_crl_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_crl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_issuer.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_issuer.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_key.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_root_cert.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_root_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/pkisecret/secret_backend_sign.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/pkisecret/secret_backend_sign.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/policy.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/provider.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/quota_lease_count.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/quota_lease_count.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/quota_rate_limit.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/quota_rate_limit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/rabbitmq/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/rabbitmq/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/raft_autopilot.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/raft_autopilot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/raft_snapshot_agent_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/raft_snapshot_agent_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/rgp_policy.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/rgp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/auth_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/saml/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/saml/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/__init__.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_association.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_aws_destination.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_aws_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_azure_destination.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_azure_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_gcp_destination.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_gcp_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_gh_destination.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_gh_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_github_apps.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_github_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/secrets/sync_vercel_destination.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/secrets/sync_vercel_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/_inputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/outputs.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/secret_backend_ca.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/secret_backend_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/ssh/secret_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/ssh/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_backend.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_creds.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/terraformcloud/secret_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/terraformcloud/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/token.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/tokenauth/auth_backend_role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/tokenauth/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/alphabet.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/alphabet.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/get_decode.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/get_decode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/get_encode.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/get_encode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/role.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/template.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/template.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transform/transformation.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transform/transformation.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/get_decrypt.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/get_decrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/get_encrypt.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/get_encrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/secret_backend_key.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault/transit/secret_cache_config.py` & `pulumi_vault-6.2.0a1715237402/pulumi_vault/transit/secret_cache_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/PKG-INFO` & `pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.2.0a1715230012
+Version: 6.2.0a1715237402
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.2.0a1715230012/pulumi_vault.egg-info/SOURCES.txt` & `pulumi_vault-6.2.0a1715237402/pulumi_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1715230012/pyproject.toml` & `pulumi_vault-6.2.0a1715237402/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_vault"
   description = "A Pulumi package for creating and managing HashiCorp Vault cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "vault"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1715230012"
+  version = "6.2.0a1715237402"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-vault"
 
 [build-system]
```

