# Comparing `tmp/stytch-9.3.1.tar.gz` & `tmp/stytch-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-9.3.1.tar", last modified: Thu Apr 25 21:33:22 2024, max compression
+gzip compressed data, was "stytch-9.4.0.tar", last modified: Fri May 10 19:42:29 2024, max compression
```

## Comparing `stytch-9.3.1.tar` & `stytch-9.4.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 21:33:08.000000 stytch-9.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-25 21:33:22.438377 stytch-9.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-25 21:33:08.000000 stytch-9.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 21:33:22.438377 stytch-9.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-25 21:33:08.000000 stytch-9.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.418377 stytch-9.3.1/stytch/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.418377 stytch-9.3.1/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.426377 stytch-9.3.1/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31578 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    52376 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    54059 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    44677 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.430377 stytch-9.3.1/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/b2b/models/totps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.430377 stytch-9.3.1/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.434377 stytch-9.3.1/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/stytch/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/lazy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/method_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/policy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/shared/rbac_local.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 21:33:08.000000 stytch-9.3.1/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-25 21:33:22.000000 stytch-9.3.1/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-25 21:33:22.000000 stytch-9.3.1/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:33:22.000000 stytch-9.3.1/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 21:33:22.000000 stytch-9.3.1/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 21:33:22.000000 stytch-9.3.1/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:33:22.438377 stytch-9.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-25 21:33:08.000000 stytch-9.3.1/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-25 21:33:08.000000 stytch-9.3.1/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 19:42:15.000000 stytch-9.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-10 19:42:29.551035 stytch-9.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-10 19:42:15.000000 stytch-9.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 19:42:29.551035 stytch-9.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-10 19:42:15.000000 stytch-9.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.531035 stytch-9.4.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.531035 stytch-9.4.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.535035 stytch-9.4.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54165 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.539035 stytch-9.4.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/totps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.543035 stytch-9.4.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.543035 stytch-9.4.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.547035 stytch-9.4.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/lazy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/method_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/policy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/rbac_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-10 19:42:15.000000 stytch-9.4.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-10 19:42:15.000000 stytch-9.4.0/test/test_integration_async.py
```

### Comparing `stytch-9.3.1/LICENSE.txt` & `stytch-9.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/PKG-INFO` & `stytch-9.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.3.1
+Version: 9.4.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.3.1/README.md` & `stytch-9.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/setup.py` & `stytch-9.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/discovery.py` & `stytch-9.4.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-9.4.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/discovery_organizations.py` & `stytch-9.4.0/stytch/b2b/api/discovery_organizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.models.discovery_organizations import CreateResponse, ListResponse
 from stytch.b2b.models.organizations import EmailImplicitRoleAssignment
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -35,15 +35,15 @@
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
         mfa_policy: Optional[str] = None,
         rbac_email_implicit_role_assignments: Optional[
-            List[EmailImplicitRoleAssignment]
+            List[Union[EmailImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         mfa_methods: Optional[str] = None,
         allowed_mfa_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
         """If an end user does not want to join any already-existing Organization, or has no possible Organizations to join, this endpoint can be used to create a new
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
@@ -161,15 +161,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
@@ -315,15 +316,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
```

### Comparing `stytch-9.3.1/stytch/b2b/api/magic_links.py` & `stytch-9.4.0/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/magic_links_discovery.py` & `stytch-9.4.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/magic_links_email.py` & `stytch-9.4.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-9.4.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/oauth.py` & `stytch-9.4.0/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/oauth_discovery.py` & `stytch-9.4.0/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/organizations.py` & `stytch-9.4.0/stytch/b2b/api/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.api.organizations_members import Members
 from stytch.b2b.models.organizations import (
     CreateResponse,
     DeleteRequestOptions,
     DeleteResponse,
     EmailImplicitRoleAssignment,
@@ -48,15 +48,15 @@
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
         mfa_policy: Optional[str] = None,
         rbac_email_implicit_role_assignments: Optional[
-            List[EmailImplicitRoleAssignment]
+            List[Union[EmailImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         mfa_methods: Optional[str] = None,
         allowed_mfa_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
         """Creates an Organization. An `organization_name` and a unique `organization_slug` are required.
 
         By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED`, and `mfa_policy` will be set to `OPTIONAL` if no Organization authentication settings are explicitly defined in the request.
@@ -145,15 +145,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/organizations", data)
@@ -267,15 +268,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/organizations", data)
@@ -331,15 +333,15 @@
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
         mfa_policy: Optional[str] = None,
         rbac_email_implicit_role_assignments: Optional[
-            List[EmailImplicitRoleAssignment]
+            List[Union[EmailImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         mfa_methods: Optional[str] = None,
         allowed_mfa_methods: Optional[List[str]] = None,
         method_options: Optional[UpdateRequestOptions] = None,
     ) -> UpdateResponse:
         """Updates an Organization specified by `organization_id`. An Organization must always have at least one auth setting set to either `RESTRICTED` or `ALL_ALLOWED` in order to provision new Members.
 
@@ -485,15 +487,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/organizations/{organization_id}", data)
@@ -667,15 +670,16 @@
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
         if mfa_policy is not None:
             data["mfa_policy"] = mfa_policy
         if rbac_email_implicit_role_assignments is not None:
             data["rbac_email_implicit_role_assignments"] = [
-                item.dict() for item in rbac_email_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in rbac_email_implicit_role_assignments
             ]
         if mfa_methods is not None:
             data["mfa_methods"] = mfa_methods
         if allowed_mfa_methods is not None:
             data["allowed_mfa_methods"] = allowed_mfa_methods
 
         url = self.api_base.url_for("/v1/b2b/organizations/{organization_id}", data)
@@ -724,15 +728,15 @@
         res = await self.async_client.delete(url, headers)
         return DeleteResponse.from_json(res.response.status, res.json)
 
     def search(
         self,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
-        query: Optional[SearchQuery] = None,
+        query: Optional[Union[SearchQuery, Dict[str, Any]]] = None,
     ) -> SearchResponse:
         """Search for Organizations. If you send a request with no body params, no filtering will be applied and the endpoint will return all Organizations. All fuzzy search filters require a minimum of three characters.
 
         Fields:
           - cursor: The `cursor` field allows you to paginate through your results. Each result array is limited to 1000 results. If your query returns more than 1000 results, you will need to paginate the responses using the `cursor`. If you receive a response that includes a non-null `next_cursor` in the `results_metadata` object, repeat the search call with the `next_cursor` value set to the `cursor` field to retrieve the next page of results. Continue to make search calls until the `next_cursor` in the response is null.
           - limit: The number of search results to return per page. The default limit is 100. A maximum of 1000 results can be returned by a single search request. If the total size of your result set is greater than one page size, you must paginate the response. See the `cursor` field.
           - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all Organizations with no filtering applied.
@@ -740,15 +744,15 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/b2b/organizations/search", data)
         res = self.sync_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status_code, res.json)
 
     async def search_async(
         self,
@@ -766,15 +770,15 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/b2b/organizations/search", data)
         res = await self.async_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status, res.json)
 
     def metrics(
         self,
```

### Comparing `stytch-9.3.1/stytch/b2b/api/organizations_members.py` & `stytch-9.4.0/stytch/b2b/api/organizations_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.api.organizations_members_oauth_providers import OAuthProviders
 from stytch.b2b.models.organizations import SearchQuery
 from stytch.b2b.models.organizations_members import (
     CreateRequestOptions,
     CreateResponse,
     DeleteMFAPhoneNumberRequestOptions,
@@ -481,15 +481,15 @@
         return DeleteTOTPResponse.from_json(res.response.status, res.json)
 
     def search(
         self,
         organization_ids: List[str],
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
-        query: Optional[SearchQuery] = None,
+        query: Optional[Union[SearchQuery, Dict[str, Any]]] = None,
         method_options: Optional[SearchRequestOptions] = None,
     ) -> SearchResponse:
         """Search for Members within specified Organizations. An array with at least one `organization_id` is required. Submitting an empty `query` returns all non-deleted Members within the specified Organizations.
 
         *All fuzzy search filters require a minimum of three characters.
 
         Our RBAC implementation offers out-of-the-box handling of authorization checks for this endpoint. If you pass in
@@ -517,15 +517,15 @@
             "organization_ids": organization_ids,
         }
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/b2b/organizations/members/search", data)
         res = self.sync_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status_code, res.json)
 
     async def search_async(
         self,
@@ -564,15 +564,15 @@
             "organization_ids": organization_ids,
         }
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/b2b/organizations/members/search", data)
         res = await self.async_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status, res.json)
 
     def delete_password(
         self,
```

### Comparing `stytch-9.3.1/stytch/b2b/api/organizations_members_oauth_providers.py` & `stytch-9.4.0/stytch/b2b/api/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/otp.py` & `stytch-9.4.0/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/otp_sms.py` & `stytch-9.4.0/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/passwords.py` & `stytch-9.4.0/stytch/b2b/api/passwords.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,19 +116,19 @@
 
     def migrate(
         self,
         email_address: str,
         hash: str,
         hash_type: Union[MigrateRequestHashType, str],
         organization_id: str,
-        md_5_config: Optional[MD5Config] = None,
-        argon_2_config: Optional[Argon2Config] = None,
-        sha_1_config: Optional[SHA1Config] = None,
-        scrypt_config: Optional[ScryptConfig] = None,
-        pbkdf_2_config: Optional[PBKDF2Config] = None,
+        md_5_config: Optional[Union[MD5Config, Dict[str, Any]]] = None,
+        argon_2_config: Optional[Union[Argon2Config, Dict[str, Any]]] = None,
+        sha_1_config: Optional[Union[SHA1Config, Dict[str, Any]]] = None,
+        scrypt_config: Optional[Union[ScryptConfig, Dict[str, Any]]] = None,
+        pbkdf_2_config: Optional[Union[PBKDF2Config, Dict[str, Any]]] = None,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         roles: Optional[List[str]] = None,
         preserve_existing_sessions: Optional[bool] = None,
     ) -> MigrateResponse:
         """Adds an existing password to a member's email that doesn't have a password yet. We support migrating members from passwords stored with bcrypt, scrypt, argon2, MD-5, SHA-1, and PBKDF2. This endpoint has a rate limit of 100 requests per second.
@@ -164,23 +164,39 @@
         data: Dict[str, Any] = {
             "email_address": email_address,
             "hash": hash,
             "hash_type": hash_type,
             "organization_id": organization_id,
         }
         if md_5_config is not None:
-            data["md_5_config"] = md_5_config.dict()
+            data["md_5_config"] = (
+                md_5_config if isinstance(md_5_config, dict) else md_5_config.dict()
+            )
         if argon_2_config is not None:
-            data["argon_2_config"] = argon_2_config.dict()
+            data["argon_2_config"] = (
+                argon_2_config
+                if isinstance(argon_2_config, dict)
+                else argon_2_config.dict()
+            )
         if sha_1_config is not None:
-            data["sha_1_config"] = sha_1_config.dict()
+            data["sha_1_config"] = (
+                sha_1_config if isinstance(sha_1_config, dict) else sha_1_config.dict()
+            )
         if scrypt_config is not None:
-            data["scrypt_config"] = scrypt_config.dict()
+            data["scrypt_config"] = (
+                scrypt_config
+                if isinstance(scrypt_config, dict)
+                else scrypt_config.dict()
+            )
         if pbkdf_2_config is not None:
-            data["pbkdf_2_config"] = pbkdf_2_config.dict()
+            data["pbkdf_2_config"] = (
+                pbkdf_2_config
+                if isinstance(pbkdf_2_config, dict)
+                else pbkdf_2_config.dict()
+            )
         if name is not None:
             data["name"] = name
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if roles is not None:
@@ -242,23 +258,39 @@
         data: Dict[str, Any] = {
             "email_address": email_address,
             "hash": hash,
             "hash_type": hash_type,
             "organization_id": organization_id,
         }
         if md_5_config is not None:
-            data["md_5_config"] = md_5_config.dict()
+            data["md_5_config"] = (
+                md_5_config if isinstance(md_5_config, dict) else md_5_config.dict()
+            )
         if argon_2_config is not None:
-            data["argon_2_config"] = argon_2_config.dict()
+            data["argon_2_config"] = (
+                argon_2_config
+                if isinstance(argon_2_config, dict)
+                else argon_2_config.dict()
+            )
         if sha_1_config is not None:
-            data["sha_1_config"] = sha_1_config.dict()
+            data["sha_1_config"] = (
+                sha_1_config if isinstance(sha_1_config, dict) else sha_1_config.dict()
+            )
         if scrypt_config is not None:
-            data["scrypt_config"] = scrypt_config.dict()
+            data["scrypt_config"] = (
+                scrypt_config
+                if isinstance(scrypt_config, dict)
+                else scrypt_config.dict()
+            )
         if pbkdf_2_config is not None:
-            data["pbkdf_2_config"] = pbkdf_2_config.dict()
+            data["pbkdf_2_config"] = (
+                pbkdf_2_config
+                if isinstance(pbkdf_2_config, dict)
+                else pbkdf_2_config.dict()
+            )
         if name is not None:
             data["name"] = name
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if roles is not None:
```

### Comparing `stytch-9.3.1/stytch/b2b/api/passwords_email.py` & `stytch-9.4.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/passwords_existing_password.py` & `stytch-9.4.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/passwords_session.py` & `stytch-9.4.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/rbac.py` & `stytch-9.4.0/stytch/b2b/api/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/recovery_codes.py` & `stytch-9.4.0/stytch/b2b/api/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/scim.py` & `stytch-9.4.0/stytch/b2b/api/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/scim_connections.py` & `stytch-9.4.0/stytch/b2b/api/scim_connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def update(
         self,
         organization_id: str,
         connection_id: str,
         display_name: Optional[str] = None,
         identity_provider: Optional[Union[UpdateRequestIdp, str]] = None,
         scim_group_implicit_role_assignments: Optional[
-            List[SCIMGroupImplicitRoleAssignments]
+            List[Union[SCIMGroupImplicitRoleAssignments, Dict[str, Any]]]
         ] = None,
         method_options: Optional[UpdateRequestOptions] = None,
     ) -> UpdateResponse:
         """Update a SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
@@ -68,15 +68,16 @@
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
             data["identity_provider"] = identity_provider
         if scim_group_implicit_role_assignments is not None:
             data["scim_group_implicit_role_assignments"] = [
-                item.dict() for item in scim_group_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in scim_group_implicit_role_assignments
             ]
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}", data
         )
         res = self.sync_client.put(url, data, headers)
         return UpdateResponse.from_json(res.response.status_code, res.json)
@@ -110,15 +111,16 @@
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
             data["identity_provider"] = identity_provider
         if scim_group_implicit_role_assignments is not None:
             data["scim_group_implicit_role_assignments"] = [
-                item.dict() for item in scim_group_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in scim_group_implicit_role_assignments
             ]
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}", data
         )
         res = await self.async_client.put(url, data, headers)
         return UpdateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.3.1/stytch/b2b/api/sessions.py` & `stytch-9.4.0/stytch/b2b/api/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def authenticate(
         self,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        authorization_check: Optional[AuthorizationCheck] = None,
+        authorization_check: Optional[Union[AuthorizationCheck, Dict[str, Any]]] = None,
     ) -> AuthenticateResponse:
         """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
         You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
 
         If an `authorization_check` object is passed in, this method will also check if the Member is authorized to perform the given action on the given Resource in the specified Organization. A Member is authorized if their Member Session contains a Role, assigned [explicitly or implicitly](https://stytch.com/docs/b2b/guides/rbac/role-assignment), with adequate permissions.
         In addition, the `organization_id` passed in the authorization check must match the Member's Organization.
@@ -144,15 +144,19 @@
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if authorization_check is not None:
-            data["authorization_check"] = authorization_check.dict()
+            data["authorization_check"] = (
+                authorization_check
+                if isinstance(authorization_check, dict)
+                else authorization_check.dict()
+            )
 
         url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
         res = self.sync_client.post(url, data, headers)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
@@ -211,15 +215,19 @@
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if authorization_check is not None:
-            data["authorization_check"] = authorization_check.dict()
+            data["authorization_check"] = (
+                authorization_check
+                if isinstance(authorization_check, dict)
+                else authorization_check.dict()
+            )
 
         url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
         res = await self.async_client.post(url, data, headers)
         return AuthenticateResponse.from_json(res.response.status, res.json)
 
     def revoke(
         self,
```

### Comparing `stytch-9.3.1/stytch/b2b/api/sso.py` & `stytch-9.4.0/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/sso_oidc.py` & `stytch-9.4.0/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/api/sso_saml.py` & `stytch-9.4.0/stytch/b2b/api/sso_saml.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.models.sso import (
     SAMLConnectionImplicitRoleAssignment,
     SAMLGroupImplicitRoleAssignment,
 )
 from stytch.b2b.models.sso_saml import (
     CreateConnectionRequestOptions,
@@ -90,18 +90,18 @@
         connection_id: str,
         idp_entity_id: Optional[str] = None,
         display_name: Optional[str] = None,
         attribute_mapping: Optional[Dict[str, Any]] = None,
         x509_certificate: Optional[str] = None,
         idp_sso_url: Optional[str] = None,
         saml_connection_implicit_role_assignments: Optional[
-            List[SAMLConnectionImplicitRoleAssignment]
+            List[Union[SAMLConnectionImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         saml_group_implicit_role_assignments: Optional[
-            List[SAMLGroupImplicitRoleAssignment]
+            List[Union[SAMLGroupImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         alternative_audience_uri: Optional[str] = None,
         method_options: Optional[UpdateConnectionRequestOptions] = None,
     ) -> UpdateConnectionResponse:
         """Updates an existing SAML connection.
 
         Note that a newly created connection will not become active until all of the following are provided:
@@ -143,19 +143,21 @@
             data["attribute_mapping"] = attribute_mapping
         if x509_certificate is not None:
             data["x509_certificate"] = x509_certificate
         if idp_sso_url is not None:
             data["idp_sso_url"] = idp_sso_url
         if saml_connection_implicit_role_assignments is not None:
             data["saml_connection_implicit_role_assignments"] = [
-                item.dict() for item in saml_connection_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in saml_connection_implicit_role_assignments
             ]
         if saml_group_implicit_role_assignments is not None:
             data["saml_group_implicit_role_assignments"] = [
-                item.dict() for item in saml_group_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in saml_group_implicit_role_assignments
             ]
         if alternative_audience_uri is not None:
             data["alternative_audience_uri"] = alternative_audience_uri
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/saml/{organization_id}/connections/{connection_id}", data
         )
@@ -221,19 +223,21 @@
             data["attribute_mapping"] = attribute_mapping
         if x509_certificate is not None:
             data["x509_certificate"] = x509_certificate
         if idp_sso_url is not None:
             data["idp_sso_url"] = idp_sso_url
         if saml_connection_implicit_role_assignments is not None:
             data["saml_connection_implicit_role_assignments"] = [
-                item.dict() for item in saml_connection_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in saml_connection_implicit_role_assignments
             ]
         if saml_group_implicit_role_assignments is not None:
             data["saml_group_implicit_role_assignments"] = [
-                item.dict() for item in saml_group_implicit_role_assignments
+                item if isinstance(item, dict) else item.dict()
+                for item in saml_group_implicit_role_assignments
             ]
         if alternative_audience_uri is not None:
             data["alternative_audience_uri"] = alternative_audience_uri
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/saml/{organization_id}/connections/{connection_id}", data
         )
```

### Comparing `stytch-9.3.1/stytch/b2b/api/totps.py` & `stytch-9.4.0/stytch/b2b/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/client.py` & `stytch-9.4.0/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/discovery.py` & `stytch-9.4.0/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-9.4.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/discovery_organizations.py` & `stytch-9.4.0/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/magic_links.py` & `stytch-9.4.0/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/magic_links_discovery.py` & `stytch-9.4.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/magic_links_email.py` & `stytch-9.4.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/mfa.py` & `stytch-9.4.0/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/oauth.py` & `stytch-9.4.0/stytch/b2b/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/oauth_discovery.py` & `stytch-9.4.0/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/organizations.py` & `stytch-9.4.0/stytch/b2b/models/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/organizations_members.py` & `stytch-9.4.0/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/organizations_members_oauth_providers.py` & `stytch-9.4.0/stytch/b2b/models/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/otp_sms.py` & `stytch-9.4.0/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/passwords.py` & `stytch-9.4.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/passwords_email.py` & `stytch-9.4.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/passwords_existing_password.py` & `stytch-9.4.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/passwords_session.py` & `stytch-9.4.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/rbac.py` & `stytch-9.4.0/stytch/b2b/models/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/recovery_codes.py` & `stytch-9.4.0/stytch/b2b/models/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/scim.py` & `stytch-9.4.0/stytch/b2b/models/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/scim_connections.py` & `stytch-9.4.0/stytch/b2b/models/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/sessions.py` & `stytch-9.4.0/stytch/b2b/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/sso.py` & `stytch-9.4.0/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/sso_oidc.py` & `stytch-9.4.0/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/sso_saml.py` & `stytch-9.4.0/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/b2b/models/totps.py` & `stytch-9.4.0/stytch/b2b/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/crypto_wallets.py` & `stytch-9.4.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/m2m.py` & `stytch-9.4.0/stytch/consumer/api/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/m2m_clients.py` & `stytch-9.4.0/stytch/consumer/api/m2m_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         res = await self.async_client.get(url, data, headers)
         return GetResponse.from_json(res.response.status, res.json)
 
     def search(
         self,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
-        query: Optional[M2MSearchQuery] = None,
+        query: Optional[Union[M2MSearchQuery, Dict[str, Any]]] = None,
     ) -> SearchResponse:
         """Search for M2M Clients within your Stytch Project. Submit an empty `query` in the request to return all M2M Clients.
 
         The following search filters are supported today:
         - `client_id`: Pass in a list of client IDs to get many clients in a single request
         - `client_name`: Search for clients by exact match on client name
         - `scopes`: Search for clients assigned a specific scope
@@ -92,15 +92,15 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/m2m/clients/search", data)
         res = self.sync_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status_code, res.json)
 
     async def search_async(
         self,
@@ -123,15 +123,15 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/m2m/clients/search", data)
         res = await self.async_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status, res.json)
 
     def update(
         self,
```

### Comparing `stytch-9.3.1/stytch/consumer/api/m2m_clients_secrets.py` & `stytch-9.4.0/stytch/consumer/api/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/magic_links.py` & `stytch-9.4.0/stytch/consumer/api/magic_links.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from stytch.consumer.api.magic_links_email import Email
 from stytch.consumer.models.attribute import Attributes
 from stytch.consumer.models.magic_links import (
     AuthenticateResponse,
     CreateResponse,
     Options,
@@ -31,16 +31,16 @@
             sync_client=self.sync_client,
             async_client=self.async_client,
         )
 
     def authenticate(
         self,
         token: str,
-        attributes: Optional[Attributes] = None,
-        options: Optional[Options] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
+        options: Optional[Union[Options, Dict[str, Any]]] = None,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
         """Authenticate a User given a Magic Link. This endpoint verifies that the Magic Link token is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
@@ -70,17 +70,19 @@
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "token": token,
         }
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
@@ -130,17 +132,19 @@
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "token": token,
         }
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
@@ -152,15 +156,15 @@
         res = await self.async_client.post(url, data, headers)
         return AuthenticateResponse.from_json(res.response.status, res.json)
 
     def create(
         self,
         user_id: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
     ) -> CreateResponse:
         """Create an embeddable Magic Link token for a User. Access to this endpoint is restricted. To enable it, please send us a note at support@stytch.com.
 
         ### Next steps
         Send the returned `token` value to the end user in a link which directs to your application. When the end user follows your link, collect the token, and call [Authenticate Magic Link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
 
         Fields:
@@ -171,15 +175,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "user_id": user_id,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
 
         url = self.api_base.url_for("/v1/magic_links", data)
         res = self.sync_client.post(url, data, headers)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
@@ -200,12 +206,14 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "user_id": user_id,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
 
         url = self.api_base.url_for("/v1/magic_links", data)
         res = await self.async_client.post(url, data, headers)
         return CreateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/magic_links_email.py` & `stytch-9.4.0/stytch/consumer/api/magic_links_email.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def send(
         self,
         email: str,
         login_template_id: Optional[str] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         login_magic_link_url: Optional[str] = None,
         signup_magic_link_url: Optional[str] = None,
         login_expiration_minutes: Optional[int] = None,
         signup_expiration_minutes: Optional[int] = None,
         code_challenge: Optional[str] = None,
         user_id: Optional[str] = None,
         session_token: Optional[str] = None,
@@ -78,15 +78,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if login_magic_link_url is not None:
             data["login_magic_link_url"] = login_magic_link_url
         if signup_magic_link_url is not None:
             data["signup_magic_link_url"] = signup_magic_link_url
         if login_expiration_minutes is not None:
             data["login_expiration_minutes"] = login_expiration_minutes
         if signup_expiration_minutes is not None:
@@ -155,15 +157,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if login_magic_link_url is not None:
             data["login_magic_link_url"] = login_magic_link_url
         if signup_magic_link_url is not None:
             data["signup_magic_link_url"] = signup_magic_link_url
         if login_expiration_minutes is not None:
             data["login_expiration_minutes"] = login_expiration_minutes
         if signup_expiration_minutes is not None:
@@ -190,15 +194,15 @@
         email: str,
         login_magic_link_url: Optional[str] = None,
         signup_magic_link_url: Optional[str] = None,
         login_expiration_minutes: Optional[int] = None,
         signup_expiration_minutes: Optional[int] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         create_user_as_pending: Optional[bool] = None,
         code_challenge: Optional[str] = None,
         locale: Optional[Union[LoginOrCreateRequestLocale, str]] = None,
     ) -> LoginOrCreateResponse:
         """Send either a login or signup Magic Link to the User based on if the email is associated with a User already. A new or pending User will receive a signup Magic Link. An active User will receive a login Magic Link. For more information on how to control the status your Users are created in see the `create_user_as_pending` flag.
 
         ### Next steps
@@ -239,15 +243,17 @@
         if signup_expiration_minutes is not None:
             data["signup_expiration_minutes"] = signup_expiration_minutes
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if signup_template_id is not None:
             data["signup_template_id"] = signup_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if code_challenge is not None:
             data["code_challenge"] = code_challenge
         if locale is not None:
             data["locale"] = locale
 
@@ -309,15 +315,17 @@
         if signup_expiration_minutes is not None:
             data["signup_expiration_minutes"] = signup_expiration_minutes
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if signup_template_id is not None:
             data["signup_template_id"] = signup_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if code_challenge is not None:
             data["code_challenge"] = code_challenge
         if locale is not None:
             data["locale"] = locale
 
@@ -325,16 +333,16 @@
         res = await self.async_client.post(url, data, headers)
         return LoginOrCreateResponse.from_json(res.response.status, res.json)
 
     def invite(
         self,
         email: str,
         invite_template_id: Optional[str] = None,
-        attributes: Optional[Attributes] = None,
-        name: Optional[Name] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
+        name: Optional[Union[Name, Dict[str, Any]]] = None,
         invite_magic_link_url: Optional[str] = None,
         invite_expiration_minutes: Optional[int] = None,
         locale: Optional[Union[InviteRequestLocale, str]] = None,
     ) -> InviteResponse:
         """Create a User and send an invite Magic Link to the provided `email`. The User will be created with a `pending` status until they click the Magic Link in the invite email.
 
         ### Next steps
@@ -357,17 +365,19 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if invite_template_id is not None:
             data["invite_template_id"] = invite_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if invite_magic_link_url is not None:
             data["invite_magic_link_url"] = invite_magic_link_url
         if invite_expiration_minutes is not None:
             data["invite_expiration_minutes"] = invite_expiration_minutes
         if locale is not None:
             data["locale"] = locale
 
@@ -407,17 +417,19 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if invite_template_id is not None:
             data["invite_template_id"] = invite_template_id
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if invite_magic_link_url is not None:
             data["invite_magic_link_url"] = invite_magic_link_url
         if invite_expiration_minutes is not None:
             data["invite_expiration_minutes"] = invite_expiration_minutes
         if locale is not None:
             data["locale"] = locale
```

### Comparing `stytch-9.3.1/stytch/consumer/api/oauth.py` & `stytch-9.4.0/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/otp.py` & `stytch-9.4.0/stytch/consumer/api/otp.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from stytch.consumer.api.otp_email import Email
 from stytch.consumer.api.otp_sms import Sms
 from stytch.consumer.api.otp_whatsapp import Whatsapp
 from stytch.consumer.models.attribute import Attributes
 from stytch.consumer.models.magic_links import Options
 from stytch.consumer.models.otp import AuthenticateResponse
@@ -41,16 +41,16 @@
             async_client=self.async_client,
         )
 
     def authenticate(
         self,
         method_id: str,
         code: str,
-        attributes: Optional[Attributes] = None,
-        options: Optional[Options] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
+        options: Optional[Union[Options, Dict[str, Any]]] = None,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
         """Authenticate a User given a `method_id` (the associated `email_id` or `phone_id`) and a `code`. This endpoint verifies that the code is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied. A given `method_id` may only have a single active OTP code at any given time, if a User requests another OTP code before the first one has expired, the first one will be invalidated.
 
@@ -76,17 +76,19 @@
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "method_id": method_id,
             "code": code,
         }
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
@@ -131,17 +133,19 @@
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "method_id": method_id,
             "code": code,
         }
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
```

### Comparing `stytch-9.3.1/stytch/consumer/api/otp_email.py` & `stytch-9.4.0/stytch/consumer/api/otp_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def send(
         self,
         email: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         locale: Optional[Union[SendRequestLocale, str]] = None,
         user_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
     ) -> SendResponse:
@@ -66,15 +66,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -127,15 +129,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -149,15 +153,15 @@
         res = await self.async_client.post(url, data, headers)
         return SendResponse.from_json(res.response.status, res.json)
 
     def login_or_create(
         self,
         email: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         create_user_as_pending: Optional[bool] = None,
         locale: Optional[Union[LoginOrCreateRequestLocale, str]] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
     ) -> LoginOrCreateResponse:
         """Send a one-time passcode (OTP) to a User using their email. If the email is not associated with a User already, a User will be created.
 
@@ -186,15 +190,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if signup_template_id is not None:
@@ -241,15 +247,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
         if login_template_id is not None:
             data["login_template_id"] = login_template_id
         if signup_template_id is not None:
```

### Comparing `stytch-9.3.1/stytch/consumer/api/otp_sms.py` & `stytch-9.4.0/stytch/consumer/api/otp_sms.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def send(
         self,
         phone_number: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         locale: Optional[Union[SendRequestLocale, str]] = None,
         user_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
     ) -> SendResponse:
         """Send a one-time passcode (OTP) to a user's phone number. If you'd like to create a user and send them a passcode with one request, use our [log in or create](https://stytch.com/docs/api/log-in-or-create-user-by-sms) endpoint.
 
@@ -73,15 +73,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -137,15 +139,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -155,15 +159,15 @@
         res = await self.async_client.post(url, data, headers)
         return SendResponse.from_json(res.response.status, res.json)
 
     def login_or_create(
         self,
         phone_number: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         create_user_as_pending: Optional[bool] = None,
         locale: Optional[Union[LoginOrCreateRequestLocale, str]] = None,
     ) -> LoginOrCreateResponse:
         """Send a One-Time Passcode (OTP) to a User using their phone number. If the phone number is not associated with a user already, a user will be created.
 
         ### Cost to send SMS OTP
         Before configuring SMS or WhatsApp OTPs, please review how Stytch [bills the costs of international OTPs](https://stytch.com/pricing) and understand how to protect your app against [toll fraud](https://stytch.com/docs/guides/passcodes/toll-fraud/overview).
@@ -195,15 +199,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
 
         url = self.api_base.url_for("/v1/otps/sms/login_or_create", data)
         res = self.sync_client.post(url, data, headers)
@@ -249,15 +255,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
 
         url = self.api_base.url_for("/v1/otps/sms/login_or_create", data)
         res = await self.async_client.post(url, data, headers)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/otp_whatsapp.py` & `stytch-9.4.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def send(
         self,
         phone_number: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         locale: Optional[Union[SendRequestLocale, str]] = None,
         user_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
     ) -> SendResponse:
         """Send a One-Time Passcode (OTP) to a User's WhatsApp. If you'd like to create a user and send them a passcode with one request, use our [log in or create](https://stytch.com/docs/api/whatsapp-login-or-create) endpoint.
 
@@ -69,15 +69,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -129,15 +131,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if locale is not None:
             data["locale"] = locale
         if user_id is not None:
             data["user_id"] = user_id
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
@@ -147,15 +151,15 @@
         res = await self.async_client.post(url, data, headers)
         return SendResponse.from_json(res.response.status, res.json)
 
     def login_or_create(
         self,
         phone_number: str,
         expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         create_user_as_pending: Optional[bool] = None,
         locale: Optional[Union[LoginOrCreateRequestLocale, str]] = None,
     ) -> LoginOrCreateResponse:
         """Send a one-time passcode (OTP) to a User's WhatsApp using their phone number. If the phone number is not associated with a User already, a User will be created.
 
         ### Cost to send SMS OTP
         Before configuring SMS or WhatsApp OTPs, please review how Stytch [bills the costs of international OTPs](https://stytch.com/pricing) and understand how to protect your app against [toll fraud](https://stytch.com/docs/guides/passcodes/toll-fraud/overview).
@@ -183,15 +187,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
 
         url = self.api_base.url_for("/v1/otps/whatsapp/login_or_create", data)
         res = self.sync_client.post(url, data, headers)
@@ -233,15 +239,17 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "phone_number": phone_number,
         }
         if expiration_minutes is not None:
             data["expiration_minutes"] = expiration_minutes
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if locale is not None:
             data["locale"] = locale
 
         url = self.api_base.url_for("/v1/otps/whatsapp/login_or_create", data)
         res = await self.async_client.post(url, data, headers)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/passwords.py` & `stytch-9.4.0/stytch/consumer/api/passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self,
         email: str,
         password: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
-        name: Optional[Name] = None,
+        name: Optional[Union[Name, Dict[str, Any]]] = None,
     ) -> CreateResponse:
         """Create a new user with a password. If `session_duration_minutes` is specified, a new session will be started as well.
 
         If a user with this email already exists in your Stytch project, this endpoint will return a `duplicate_email` error. To add a password to an existing passwordless user, you'll need to either call the [Migrate password endpoint](https://stytch.com/docs/api/password-migrate) or prompt the user to complete one of our password reset flows.
 
         This endpoint will return an error if the password provided does not meet our strength requirements, which you can check beforehand via the [Password strength check endpoint](https://stytch.com/docs/api/password-strength-check).
 
@@ -98,15 +98,15 @@
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
 
         url = self.api_base.url_for("/v1/passwords", data)
         res = self.sync_client.post(url, data, headers)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
@@ -155,15 +155,15 @@
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
 
         url = self.api_base.url_for("/v1/passwords", data)
         res = await self.async_client.post(url, data, headers)
         return CreateResponse.from_json(res.response.status, res.json)
 
     def authenticate(
         self,
@@ -338,23 +338,23 @@
         return StrengthCheckResponse.from_json(res.response.status, res.json)
 
     def migrate(
         self,
         email: str,
         hash: str,
         hash_type: Union[MigrateRequestHashType, str],
-        md_5_config: Optional[MD5Config] = None,
-        argon_2_config: Optional[Argon2Config] = None,
-        sha_1_config: Optional[SHA1Config] = None,
-        scrypt_config: Optional[ScryptConfig] = None,
-        pbkdf_2_config: Optional[PBKDF2Config] = None,
+        md_5_config: Optional[Union[MD5Config, Dict[str, Any]]] = None,
+        argon_2_config: Optional[Union[Argon2Config, Dict[str, Any]]] = None,
+        sha_1_config: Optional[Union[SHA1Config, Dict[str, Any]]] = None,
+        scrypt_config: Optional[Union[ScryptConfig, Dict[str, Any]]] = None,
+        pbkdf_2_config: Optional[Union[PBKDF2Config, Dict[str, Any]]] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         set_email_verified: Optional[bool] = None,
-        name: Optional[Name] = None,
+        name: Optional[Union[Name, Dict[str, Any]]] = None,
     ) -> MigrateResponse:
         """Adds an existing password to a User's email that doesn't have a password yet. We support migrating users from passwords stored with `bcrypt`, `scrypt`, `argon2`, `MD-5`, `SHA-1`, or `PBKDF2`. This endpoint has a rate limit of 100 requests per second.
 
         Fields:
           - email: The email address of the end user.
           - hash: The password hash. For a Scrypt or PBKDF2 hash, the hash needs to be a base64 encoded string.
           - hash_type: The password hash used. Currently `bcrypt`, `scrypt`, `argon_2i`, `argon_2id`, `md_5`, `sha_1`, and `pbkdf_2` are supported.
@@ -373,31 +373,47 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
             "hash": hash,
             "hash_type": hash_type,
         }
         if md_5_config is not None:
-            data["md_5_config"] = md_5_config.dict()
+            data["md_5_config"] = (
+                md_5_config if isinstance(md_5_config, dict) else md_5_config.dict()
+            )
         if argon_2_config is not None:
-            data["argon_2_config"] = argon_2_config.dict()
+            data["argon_2_config"] = (
+                argon_2_config
+                if isinstance(argon_2_config, dict)
+                else argon_2_config.dict()
+            )
         if sha_1_config is not None:
-            data["sha_1_config"] = sha_1_config.dict()
+            data["sha_1_config"] = (
+                sha_1_config if isinstance(sha_1_config, dict) else sha_1_config.dict()
+            )
         if scrypt_config is not None:
-            data["scrypt_config"] = scrypt_config.dict()
+            data["scrypt_config"] = (
+                scrypt_config
+                if isinstance(scrypt_config, dict)
+                else scrypt_config.dict()
+            )
         if pbkdf_2_config is not None:
-            data["pbkdf_2_config"] = pbkdf_2_config.dict()
+            data["pbkdf_2_config"] = (
+                pbkdf_2_config
+                if isinstance(pbkdf_2_config, dict)
+                else pbkdf_2_config.dict()
+            )
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if set_email_verified is not None:
             data["set_email_verified"] = set_email_verified
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
 
         url = self.api_base.url_for("/v1/passwords/migrate", data)
         res = self.sync_client.post(url, data, headers)
         return MigrateResponse.from_json(res.response.status_code, res.json)
 
     async def migrate_async(
         self,
@@ -435,28 +451,44 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "email": email,
             "hash": hash,
             "hash_type": hash_type,
         }
         if md_5_config is not None:
-            data["md_5_config"] = md_5_config.dict()
+            data["md_5_config"] = (
+                md_5_config if isinstance(md_5_config, dict) else md_5_config.dict()
+            )
         if argon_2_config is not None:
-            data["argon_2_config"] = argon_2_config.dict()
+            data["argon_2_config"] = (
+                argon_2_config
+                if isinstance(argon_2_config, dict)
+                else argon_2_config.dict()
+            )
         if sha_1_config is not None:
-            data["sha_1_config"] = sha_1_config.dict()
+            data["sha_1_config"] = (
+                sha_1_config if isinstance(sha_1_config, dict) else sha_1_config.dict()
+            )
         if scrypt_config is not None:
-            data["scrypt_config"] = scrypt_config.dict()
+            data["scrypt_config"] = (
+                scrypt_config
+                if isinstance(scrypt_config, dict)
+                else scrypt_config.dict()
+            )
         if pbkdf_2_config is not None:
-            data["pbkdf_2_config"] = pbkdf_2_config.dict()
+            data["pbkdf_2_config"] = (
+                pbkdf_2_config
+                if isinstance(pbkdf_2_config, dict)
+                else pbkdf_2_config.dict()
+            )
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if set_email_verified is not None:
             data["set_email_verified"] = set_email_verified
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
 
         url = self.api_base.url_for("/v1/passwords/migrate", data)
         res = await self.async_client.post(url, data, headers)
         return MigrateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/passwords_email.py` & `stytch-9.4.0/stytch/consumer/api/passwords_email.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def reset_start(
         self,
         email: str,
         reset_password_redirect_url: Optional[str] = None,
         reset_password_expiration_minutes: Optional[int] = None,
         code_challenge: Optional[str] = None,
-        attributes: Optional[Attributes] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         login_redirect_url: Optional[str] = None,
         locale: Optional[Union[ResetStartRequestLocale, str]] = None,
         reset_password_template_id: Optional[str] = None,
     ) -> ResetStartResponse:
         """Initiates a password reset for the email address provided. This will trigger an email to be sent to the address, containing a magic link that will allow them to set a new password and authenticate.
 
         Fields:
@@ -72,15 +72,17 @@
         if reset_password_expiration_minutes is not None:
             data[
                 "reset_password_expiration_minutes"
             ] = reset_password_expiration_minutes
         if code_challenge is not None:
             data["code_challenge"] = code_challenge
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if login_redirect_url is not None:
             data["login_redirect_url"] = login_redirect_url
         if locale is not None:
             data["locale"] = locale
         if reset_password_template_id is not None:
             data["reset_password_template_id"] = reset_password_template_id
 
@@ -133,15 +135,17 @@
         if reset_password_expiration_minutes is not None:
             data[
                 "reset_password_expiration_minutes"
             ] = reset_password_expiration_minutes
         if code_challenge is not None:
             data["code_challenge"] = code_challenge
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if login_redirect_url is not None:
             data["login_redirect_url"] = login_redirect_url
         if locale is not None:
             data["locale"] = locale
         if reset_password_template_id is not None:
             data["reset_password_template_id"] = reset_password_template_id
 
@@ -154,16 +158,16 @@
         token: str,
         password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         code_verifier: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        attributes: Optional[Attributes] = None,
-        options: Optional[Options] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
+        options: Optional[Union[Options, Dict[str, Any]]] = None,
     ) -> ResetResponse:
         """Reset the user’s password and authenticate them. This endpoint checks that the magic link `token` is valid, hasn’t expired, or already been used – and can optionally require additional security settings, such as the IP address and user agent matching the initial reset request.
 
         The provided password needs to meet our password strength requirements, which can be checked in advance with the password strength endpoint. If the token and password are accepted, the password is securely stored for future authentication and the user is authenticated.
 
         Note that a successful password reset by email will revoke all active sessions for the `user_id`.
 
@@ -204,17 +208,19 @@
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
 
         url = self.api_base.url_for("/v1/passwords/email/reset", data)
         res = self.sync_client.post(url, data, headers)
         return ResetResponse.from_json(res.response.status_code, res.json)
 
     async def reset_async(
         self,
@@ -271,14 +277,16 @@
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if options is not None:
-            data["options"] = options.dict()
+            data["options"] = options if isinstance(options, dict) else options.dict()
 
         url = self.api_base.url_for("/v1/passwords/email/reset", data)
         res = await self.async_client.post(url, data, headers)
         return ResetResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/passwords_existing_password.py` & `stytch-9.4.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/passwords_session.py` & `stytch-9.4.0/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/project.py` & `stytch-9.4.0/stytch/consumer/api/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/sessions.py` & `stytch-9.4.0/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/totps.py` & `stytch-9.4.0/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/api/users.py` & `stytch-9.4.0/stytch/consumer/api/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, AsyncGenerator, Dict, Generator, Optional
+from typing import Any, AsyncGenerator, Dict, Generator, Optional, Union
 
 from stytch.consumer.models.attribute import Attributes
 from stytch.consumer.models.users import (
     CreateResponse,
     DeleteBiometricRegistrationResponse,
     DeleteCryptoWalletResponse,
     DeleteEmailResponse,
@@ -38,16 +38,16 @@
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
     def create(
         self,
         email: Optional[str] = None,
-        name: Optional[Name] = None,
-        attributes: Optional[Attributes] = None,
+        name: Optional[Union[Name, Dict[str, Any]]] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         phone_number: Optional[str] = None,
         create_user_as_pending: Optional[bool] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
     ) -> CreateResponse:
         """Add a User to Stytch. A `user_id` is returned in the response that can then be used to perform other operations within Stytch. An `email` or a `phone_number` is required.
 
@@ -65,17 +65,19 @@
           - untrusted_metadata: The `untrusted_metadata` field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end users directly via the SDK, and **cannot be used to store critical information.** See the [Metadata](https://stytch.com/docs/api/metadata) reference for complete field behavior details.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if email is not None:
             data["email"] = email
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if phone_number is not None:
             data["phone_number"] = phone_number
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
@@ -111,17 +113,19 @@
           - untrusted_metadata: The `untrusted_metadata` field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end users directly via the SDK, and **cannot be used to store critical information.** See the [Metadata](https://stytch.com/docs/api/metadata) reference for complete field behavior details.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if email is not None:
             data["email"] = email
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if phone_number is not None:
             data["phone_number"] = phone_number
         if create_user_as_pending is not None:
             data["create_user_as_pending"] = create_user_as_pending
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
@@ -167,15 +171,15 @@
         res = await self.async_client.get(url, data, headers)
         return GetResponse.from_json(res.response.status, res.json)
 
     def search(
         self,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
-        query: Optional[SearchUsersQuery] = None,
+        query: Optional[Union[SearchUsersQuery, Dict[str, Any]]] = None,
     ) -> SearchResponse:
         """Search for Users within your Stytch Project. Submit an empty `query` in the request to return all Users.
 
         Fields:
           - cursor: The `cursor` field allows you to paginate through your results. Each result array is limited to 1000 results. If your query returns more than 1000 results, you will need to paginate the responses using the `cursor`. If you receive a response that includes a non-null `next_cursor` in the `results_metadata` object, repeat the search call with the `next_cursor` value set to the `cursor` field to retrieve the next page of results. Continue to make search calls until the `next_cursor` in the response is null.
           - limit: The number of search results to return per page. The default limit is 100. A maximum of 1000 results can be returned by a single search request. If the total size of your result set is greater than one page size, you must paginate the response. See the `cursor` field.
           - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all results with no filtering applied.
@@ -183,15 +187,15 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/users/search", data)
         res = self.sync_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status_code, res.json)
 
     async def search_async(
         self,
@@ -209,25 +213,25 @@
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {}
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
             data["limit"] = limit
         if query is not None:
-            data["query"] = query.dict()
+            data["query"] = query if isinstance(query, dict) else query.dict()
 
         url = self.api_base.url_for("/v1/users/search", data)
         res = await self.async_client.post(url, data, headers)
         return SearchResponse.from_json(res.response.status, res.json)
 
     def update(
         self,
         user_id: str,
-        name: Optional[Name] = None,
-        attributes: Optional[Attributes] = None,
+        name: Optional[Union[Name, Dict[str, Any]]] = None,
+        attributes: Optional[Union[Attributes, Dict[str, Any]]] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
     ) -> UpdateResponse:
         """Update a User's attributes.
 
         **Note:** In order to add a new email address or phone number to an existing User object, pass the new email address or phone number into the respective `/send` endpoint for the authentication method of your choice. If you specify the existing User's `user_id` while calling the `/send` endpoint, the new, unverified email address or phone number will be added to the existing User object. If the user successfully authenticates within 5 minutes of the `/send` request, the new email address or phone number will be marked as verified and remain permanently on the existing Stytch User. Otherwise, it will be removed from the User object, and any subsequent login requests using that phone number will create a new User. We require this process to guard against an account takeover vulnerability.
 
@@ -239,17 +243,19 @@
           - untrusted_metadata: The `untrusted_metadata` field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end users directly via the SDK, and **cannot be used to store critical information.** See the [Metadata](https://stytch.com/docs/api/metadata) reference for complete field behavior details.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "user_id": user_id,
         }
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
 
         url = self.api_base.url_for("/v1/users/{user_id}", data)
         res = self.sync_client.put(url, data, headers)
@@ -275,17 +281,19 @@
           - untrusted_metadata: The `untrusted_metadata` field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end users directly via the SDK, and **cannot be used to store critical information.** See the [Metadata](https://stytch.com/docs/api/metadata) reference for complete field behavior details.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "user_id": user_id,
         }
         if name is not None:
-            data["name"] = name.dict()
+            data["name"] = name if isinstance(name, dict) else name.dict()
         if attributes is not None:
-            data["attributes"] = attributes.dict()
+            data["attributes"] = (
+                attributes if isinstance(attributes, dict) else attributes.dict()
+            )
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
 
         url = self.api_base.url_for("/v1/users/{user_id}", data)
         res = await self.async_client.put(url, data, headers)
```

### Comparing `stytch-9.3.1/stytch/consumer/api/webauthn.py` & `stytch-9.4.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/client.py` & `stytch-9.4.0/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/crypto_wallets.py` & `stytch-9.4.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/m2m.py` & `stytch-9.4.0/stytch/consumer/models/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/m2m_clients.py` & `stytch-9.4.0/stytch/consumer/models/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/m2m_clients_secrets.py` & `stytch-9.4.0/stytch/consumer/models/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/magic_links.py` & `stytch-9.4.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/magic_links_email.py` & `stytch-9.4.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/oauth.py` & `stytch-9.4.0/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/otp.py` & `stytch-9.4.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/otp_email.py` & `stytch-9.4.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/otp_sms.py` & `stytch-9.4.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/otp_whatsapp.py` & `stytch-9.4.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/passwords.py` & `stytch-9.4.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/passwords_email.py` & `stytch-9.4.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/passwords_existing_password.py` & `stytch-9.4.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/passwords_session.py` & `stytch-9.4.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/project.py` & `stytch-9.4.0/stytch/consumer/models/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/sessions.py` & `stytch-9.4.0/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/totps.py` & `stytch-9.4.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/users.py` & `stytch-9.4.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/consumer/models/webauthn.py` & `stytch-9.4.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/core/api_base.py` & `stytch-9.4.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/core/client_base.py` & `stytch-9.4.0/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/core/http/client.py` & `stytch-9.4.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/core/response_base.py` & `stytch-9.4.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/shared/jwt_helpers.py` & `stytch-9.4.0/stytch/shared/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/shared/lazy_cache.py` & `stytch-9.4.0/stytch/shared/lazy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/shared/method_options.py` & `stytch-9.4.0/stytch/shared/method_options.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/shared/policy_cache.py` & `stytch-9.4.0/stytch/shared/policy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch/shared/rbac_local.py` & `stytch-9.4.0/stytch/shared/rbac_local.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/stytch.egg-info/PKG-INFO` & `stytch-9.4.0/stytch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.3.1
+Version: 9.4.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.3.1/stytch.egg-info/SOURCES.txt` & `stytch-9.4.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/test/test_integration.py` & `stytch-9.4.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-9.3.1/test/test_integration_async.py` & `stytch-9.4.0/test/test_integration_async.py`

 * *Files identical despite different names*

