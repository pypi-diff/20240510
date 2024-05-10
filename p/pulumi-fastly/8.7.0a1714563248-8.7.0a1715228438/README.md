# Comparing `tmp/pulumi_fastly-8.7.0a1714563248.tar.gz` & `tmp/pulumi_fastly-8.7.0a1715228438.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.7.0a1714563248.tar", last modified: Wed May  1 11:39:37 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.7.0a1715228438.tar", last modified: Thu May  9 04:25:47 2024, max compression
```

## Comparing `pulumi_fastly-8.7.0a1714563248.tar` & `pulumi_fastly-8.7.0a1715228438.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:39:37.561641 pulumi_fastly-8.7.0a1714563248/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-01 11:39:37.561641 pulumi_fastly-8.7.0a1714563248/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:39:37.557641 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:39:37.561641 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_vcl_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97303 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   126107 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:39:37.561641 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-01 11:39:37.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-01 11:39:37.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:39:37.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 11:39:37.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 11:39:37.000000 pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-01 11:39:31.000000 pulumi_fastly-8.7.0a1714563248/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:39:37.561641 pulumi_fastly-8.7.0a1714563248/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_vcl_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97303 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126107 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/setup.cfg
```

### Comparing `pulumi_fastly-8.7.0a1714563248/PKG-INFO` & `pulumi_fastly-8.7.0a1715228438/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1714563248
+Version: 8.7.0a1715228438
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1714563248/README.md` & `pulumi_fastly-8.7.0a1715228438/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/__init__.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/alert.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/configstore.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_services.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_vcl_snippets.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_vcl_snippets.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/outputs.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/provider.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly/user.py` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1714563248
+Version: 8.7.0a1715228438
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1714563248/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1714563248/pyproject.toml` & `pulumi_fastly-8.7.0a1715228438/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.7.0a1714563248"
+  version = "8.7.0a1715228438"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

