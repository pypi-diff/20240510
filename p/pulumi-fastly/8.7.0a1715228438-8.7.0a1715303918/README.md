# Comparing `tmp/pulumi_fastly-8.7.0a1715228438.tar.gz` & `tmp/pulumi_fastly-8.7.0a1715303918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.7.0a1715228438.tar", last modified: Thu May  9 04:25:47 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.7.0a1715303918.tar", last modified: Fri May 10 01:31:40 2024, max compression
```

## Comparing `pulumi_fastly-8.7.0a1715228438.tar` & `pulumi_fastly-8.7.0a1715303918.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_vcl_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97303 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   126107 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 04:25:47.000000 pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-09 04:25:41.000000 pulumi_fastly-8.7.0a1715228438/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:25:47.835470 pulumi_fastly-8.7.0a1715228438/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_vcl_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92401 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121205 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20467 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/setup.cfg
```

### Comparing `pulumi_fastly-8.7.0a1715228438/PKG-INFO` & `pulumi_fastly-8.7.0a1715303918/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1715228438
+Version: 8.7.0a1715303918
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1715228438/README.md` & `pulumi_fastly-8.7.0a1715303918/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/__init__.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/alert.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore_entries.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,14 @@
                  entries: pulumi.Input[Mapping[str, Any]],
                  store_id: pulumi.Input[str],
                  manage_entries: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ConfigstoreEntries resource.
         :param pulumi.Input[Mapping[str, Any]] entries: A map representing an entry in the Config Store, (key/value)
         :param pulumi.Input[str] store_id: An alphanumeric string identifying the Config Store.
-        :param pulumi.Input[bool] manage_entries: Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-               externally from the config seeded values.
         """
         pulumi.set(__self__, "entries", entries)
         pulumi.set(__self__, "store_id", store_id)
         if manage_entries is not None:
             pulumi.set(__self__, "manage_entries", manage_entries)
 
     @property
@@ -52,18 +50,14 @@
     @store_id.setter
     def store_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "store_id", value)
 
     @property
     @pulumi.getter(name="manageEntries")
     def manage_entries(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-        externally from the config seeded values.
-        """
         return pulumi.get(self, "manage_entries")
 
     @manage_entries.setter
     def manage_entries(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "manage_entries", value)
 
 
@@ -72,16 +66,14 @@
     def __init__(__self__, *,
                  entries: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  manage_entries: Optional[pulumi.Input[bool]] = None,
                  store_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ConfigstoreEntries resources.
         :param pulumi.Input[Mapping[str, Any]] entries: A map representing an entry in the Config Store, (key/value)
-        :param pulumi.Input[bool] manage_entries: Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-               externally from the config seeded values.
         :param pulumi.Input[str] store_id: An alphanumeric string identifying the Config Store.
         """
         if entries is not None:
             pulumi.set(__self__, "entries", entries)
         if manage_entries is not None:
             pulumi.set(__self__, "manage_entries", manage_entries)
         if store_id is not None:
@@ -98,18 +90,14 @@
     @entries.setter
     def entries(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "entries", value)
 
     @property
     @pulumi.getter(name="manageEntries")
     def manage_entries(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-        externally from the config seeded values.
-        """
         return pulumi.get(self, "manage_entries")
 
     @manage_entries.setter
     def manage_entries(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "manage_entries", value)
 
     @property
@@ -142,16 +130,14 @@
         ```sh
         $ pulumi import fastly:index/configstoreEntries:ConfigstoreEntries example xxxxxxxxxxxxxxxxxxxx/entries
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] entries: A map representing an entry in the Config Store, (key/value)
-        :param pulumi.Input[bool] manage_entries: Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-               externally from the config seeded values.
         :param pulumi.Input[str] store_id: An alphanumeric string identifying the Config Store.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConfigstoreEntriesArgs,
@@ -216,16 +202,14 @@
         Get an existing ConfigstoreEntries resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] entries: A map representing an entry in the Config Store, (key/value)
-        :param pulumi.Input[bool] manage_entries: Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-               externally from the config seeded values.
         :param pulumi.Input[str] store_id: An alphanumeric string identifying the Config Store.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConfigstoreEntriesState.__new__(_ConfigstoreEntriesState)
 
         __props__.__dict__["entries"] = entries
@@ -240,18 +224,14 @@
         A map representing an entry in the Config Store, (key/value)
         """
         return pulumi.get(self, "entries")
 
     @property
     @pulumi.getter(name="manageEntries")
     def manage_entries(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Have Terraform manage the entries (default: false). If set to `true` Terraform will remove any entries that were added
-        externally from the config seeded values.
-        """
         return pulumi.get(self, "manage_entries")
 
     @property
     @pulumi.getter(name="storeId")
     def store_id(self) -> pulumi.Output[str]:
         """
         An alphanumeric string identifying the Config Store.
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_services.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_vcl_snippets.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_vcl_snippets.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/outputs.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/provider.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] api_key: Fastly API Key from https://app.fastly.com/#account
         :param pulumi.Input[str] base_url: Fastly API URL
         :param pulumi.Input[bool] force_http2: Set this to `true` to disable HTTP/1.x fallback mechanism that the underlying Go library will attempt upon connection to
                `api.fastly.com:443` by default. This may slightly improve the provider's performance and reduce unnecessary TLS
                handshakes. Default: `false`
         :param pulumi.Input[bool] no_auth: Set to `true` if your configuration only consumes data sources that do not require authentication, such as
-               `fastly_ip_ranges`
+               `get_fastly_ip_ranges`
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if base_url is not None:
             pulumi.set(__self__, "base_url", base_url)
         if force_http2 is not None:
             pulumi.set(__self__, "force_http2", force_http2)
@@ -76,15 +76,15 @@
         pulumi.set(self, "force_http2", value)
 
     @property
     @pulumi.getter(name="noAuth")
     def no_auth(self) -> Optional[pulumi.Input[bool]]:
         """
         Set to `true` if your configuration only consumes data sources that do not require authentication, such as
-        `fastly_ip_ranges`
+        `get_fastly_ip_ranges`
         """
         return pulumi.get(self, "no_auth")
 
     @no_auth.setter
     def no_auth(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "no_auth", value)
 
@@ -109,15 +109,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_key: Fastly API Key from https://app.fastly.com/#account
         :param pulumi.Input[str] base_url: Fastly API URL
         :param pulumi.Input[bool] force_http2: Set this to `true` to disable HTTP/1.x fallback mechanism that the underlying Go library will attempt upon connection to
                `api.fastly.com:443` by default. This may slightly improve the provider's performance and reduce unnecessary TLS
                handshakes. Default: `false`
         :param pulumi.Input[bool] no_auth: Set to `true` if your configuration only consumes data sources that do not require authentication, such as
-               `fastly_ip_ranges`
+               `get_fastly_ip_ranges`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,22 +54,18 @@
                  resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ServiceCompute resource.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         pulumi.set(__self__, "domains", domains)
         if activate is not None:
             pulumi.set(__self__, "activate", activate)
         if backends is not None:
             pulumi.set(__self__, "backends", backends)
@@ -176,17 +172,14 @@
     @backends.setter
     def backends(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeBackendArgs']]]]):
         pulumi.set(self, "backends", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
@@ -488,19 +481,14 @@
     @resource_links.setter
     def resource_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]):
         pulumi.set(self, "resource_links", value)
 
     @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @reuse.setter
     def reuse(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reuse", value)
 
     @property
@@ -562,27 +550,20 @@
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ServiceCompute resources.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-               local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-               UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         if activate is not None:
             pulumi.set(__self__, "activate", activate)
         if active_version is not None:
             pulumi.set(__self__, "active_version", active_version)
         if backends is not None:
@@ -710,17 +691,14 @@
     @cloned_version.setter
     def cloned_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloned_version", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
@@ -755,19 +733,14 @@
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-        local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-        UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        """
         return pulumi.get(self, "force_refresh")
 
     @force_refresh.setter
     def force_refresh(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_refresh", value)
 
     @property
@@ -1060,19 +1033,14 @@
     @resource_links.setter
     def resource_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]):
         pulumi.set(self, "resource_links", value)
 
     @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @reuse.setter
     def reuse(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reuse", value)
 
     @property
@@ -1148,23 +1116,19 @@
         ```sh
         $ pulumi import fastly:index/serviceCompute:ServiceCompute demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceComputeArgs,
@@ -1350,27 +1314,20 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-               local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-               UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceComputeState.__new__(_ServiceComputeState)
 
         __props__.__dict__["activate"] = activate
@@ -1445,17 +1402,14 @@
         The latest cloned version by the provider
         """
         return pulumi.get(self, "cloned_version")
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def dictionaries(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceComputeDictionary']]]:
         return pulumi.get(self, "dictionaries")
 
@@ -1474,19 +1428,14 @@
         Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
-        """
-        Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-        local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-        UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        """
         return pulumi.get(self, "force_refresh")
 
     @property
     @pulumi.getter
     def imported(self) -> pulumi.Output[bool]:
         """
         Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
@@ -1651,19 +1600,14 @@
         A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         """
         return pulumi.get(self, "resource_links")
 
     @property
     @pulumi.getter
     def reuse(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @property
     @pulumi.getter(name="versionComment")
     def version_comment(self) -> pulumi.Output[Optional[str]]:
         """
         Description field for the version
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_vcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,23 +72,19 @@
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         The set of arguments for constructing a ServiceVcl resource.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         pulumi.set(__self__, "domains", domains)
         if acls is not None:
             pulumi.set(__self__, "acls", acls)
@@ -251,17 +247,14 @@
     @cache_settings.setter
     def cache_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclCacheSettingArgs']]]]):
         pulumi.set(self, "cache_settings", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
@@ -665,19 +658,14 @@
     @response_objects.setter
     def response_objects(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]):
         pulumi.set(self, "response_objects", value)
 
     @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @reuse.setter
     def reuse(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reuse", value)
 
     @property
@@ -808,28 +796,21 @@
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         Input properties used for looking up and filtering ServiceVcl resources.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-               local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-               UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         if acls is not None:
             pulumi.set(__self__, "acls", acls)
         if activate is not None:
@@ -1013,17 +994,14 @@
     @cloned_version.setter
     def cloned_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloned_version", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
@@ -1109,19 +1087,14 @@
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-        local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-        UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        """
         return pulumi.get(self, "force_refresh")
 
     @force_refresh.setter
     def force_refresh(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_refresh", value)
 
     @property
@@ -1465,19 +1438,14 @@
     @response_objects.setter
     def response_objects(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]):
         pulumi.set(self, "response_objects", value)
 
     @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @reuse.setter
     def reuse(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reuse", value)
 
     @property
@@ -1622,24 +1590,20 @@
         ```sh
         $ pulumi import fastly:index/serviceVcl:ServiceVcl demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         ...
     @overload
     def __init__(__self__,
@@ -1881,28 +1845,21 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-               local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-               UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-               deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-               an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceVclState.__new__(_ServiceVclState)
@@ -2007,17 +1964,14 @@
         The latest cloned version by the provider
         """
         return pulumi.get(self, "cloned_version")
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
-        """
-        Description field for the service. Default `Managed by Terraform`
-        """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def conditions(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclCondition']]]:
         return pulumi.get(self, "conditions")
 
@@ -2067,19 +2021,14 @@
         Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
-        """
-        Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
-        local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
-        UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        """
         return pulumi.get(self, "force_refresh")
 
     @property
     @pulumi.getter
     def gzips(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclGzip']]]:
         return pulumi.get(self, "gzips")
 
@@ -2271,19 +2220,14 @@
     @pulumi.getter(name="responseObjects")
     def response_objects(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclResponseObject']]]:
         return pulumi.get(self, "response_objects")
 
     @property
     @pulumi.getter
     def reuse(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
-        deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
-        an active service will cause an error. Default `false`
-        """
         return pulumi.get(self, "reuse")
 
     @property
     @pulumi.getter
     def snippets(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclSnippet']]]:
         return pulumi.get(self, "snippets")
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_mutual_authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,14 @@
                  include: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a TlsMutualAuthentication resource.
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         """
         pulumi.set(__self__, "cert_bundle", cert_bundle)
         if activation_ids is not None:
             pulumi.set(__self__, "activation_ids", activation_ids)
         if enforced is not None:
             pulumi.set(__self__, "enforced", enforced)
@@ -73,18 +71,14 @@
     @enforced.setter
     def enforced(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enforced", value)
 
     @property
     @pulumi.getter
     def include(self) -> Optional[pulumi.Input[str]]:
-        """
-        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-        authentication from the Fastly API (permitted values: `tls_activations`).
-        """
         return pulumi.get(self, "include")
 
     @include.setter
     def include(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "include", value)
 
     @property
@@ -113,16 +107,14 @@
                  updated_at: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TlsMutualAuthentication resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[str] created_at: Date and time in ISO 8601 format.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tls_activations: List of alphanumeric strings identifying TLS activations.
         :param pulumi.Input[str] updated_at: Date and time in ISO 8601 format.
         """
         if activation_ids is not None:
             pulumi.set(__self__, "activation_ids", activation_ids)
         if cert_bundle is not None:
@@ -187,18 +179,14 @@
     @enforced.setter
     def enforced(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enforced", value)
 
     @property
     @pulumi.getter
     def include(self) -> Optional[pulumi.Input[str]]:
-        """
-        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-        authentication from the Fastly API (permitted values: `tls_activations`).
-        """
         return pulumi.get(self, "include")
 
     @include.setter
     def include(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "include", value)
 
     @property
@@ -259,16 +247,14 @@
         The examples below demonstrate how to use Mutual Authentication along with a TLS Subscription. Refer to the `TlsSubscription` resource documentation for a deeper explanation of that code.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TlsMutualAuthenticationArgs,
@@ -346,16 +332,14 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[str] created_at: Date and time in ISO 8601 format.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tls_activations: List of alphanumeric strings identifying TLS activations.
         :param pulumi.Input[str] updated_at: Date and time in ISO 8601 format.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TlsMutualAuthenticationState.__new__(_TlsMutualAuthenticationState)
@@ -401,18 +385,14 @@
         Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
         """
         return pulumi.get(self, "enforced")
 
     @property
     @pulumi.getter
     def include(self) -> pulumi.Output[Optional[str]]:
-        """
-        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
-        authentication from the Fastly API (permitted values: `tls_activations`).
-        """
         return pulumi.get(self, "include")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly/user.py` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1715228438
+Version: 8.7.0a1715303918
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1715228438/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715228438/pyproject.toml` & `pulumi_fastly-8.7.0a1715303918/pyproject.toml`

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
-  version = "8.7.0a1715228438"
+  version = "8.7.0a1715303918"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

