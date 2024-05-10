# Comparing `tmp/neon-skill-ip_address-1.2.1a2.tar.gz` & `tmp/neon-skill-ip_address-1.2.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-ip_address-1.2.1a2.tar", last modified: Mon Apr 29 17:44:44 2024, max compression
+gzip compressed data, was "neon-skill-ip_address-1.2.1a3.tar", last modified: Fri May 10 17:37:24 2024, max compression
```

## Comparing `neon-skill-ip_address-1.2.1a2.tar` & `neon-skill-ip_address-1.2.1a3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.376563 neon-skill-ip_address-1.2.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/public.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/word_local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/word_public.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/locale/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/ethernet.connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/last digits device.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/last digits.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/public.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/word_local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/word_public.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.167588 neon-skill-ip_address-1.2.1a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.167588 neon-skill-ip_address-1.2.1a3/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/ca-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.171588 neon-skill-ip_address-1.2.1a3/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/cs-cz/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.171588 neon-skill-ip_address-1.2.1a3/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/de-de/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.171588 neon-skill-ip_address-1.2.1a3/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/public.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/word_local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/en-us/word_public.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.171588 neon-skill-ip_address-1.2.1a3/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/es-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.171588 neon-skill-ip_address-1.2.1a3/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/eu-eu/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.175588 neon-skill-ip_address-1.2.1a3/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/it-it/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.175588 neon-skill-ip_address-1.2.1a3/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pl-pl/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.175588 neon-skill-ip_address-1.2.1a3/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/pt-br/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.175588 neon-skill-ip_address-1.2.1a3/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/sv-se/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/locale/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/ethernet.connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/last digits device.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/last digits.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/public.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/word_local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/locale/uk-ua/word_public.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 17:37:24.000000 neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:37:24.179588 neon-skill-ip_address-1.2.1a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 17:37:21.000000 neon-skill-ip_address-1.2.1a3/version.py
```

### Comparing `neon-skill-ip_address-1.2.1a2/LICENSE` & `neon-skill-ip_address-1.2.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/LICENSE.md` & `neon-skill-ip_address-1.2.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/PKG-INFO` & `neon-skill-ip_address-1.2.1a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip_address
-Version: 1.2.1a2
+Version: 1.2.1a3
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-ip_address-1.2.1a2/README.md` & `neon-skill-ip_address-1.2.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/__init__.py` & `neon-skill-ip_address-1.2.1a3/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/PKG-INFO` & `neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip-address
-Version: 1.2.1a2
+Version: 1.2.1a3
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/SOURCES.txt` & `neon-skill-ip_address-1.2.1a3/neon_skill_ip_address.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/setup.py` & `neon-skill-ip_address-1.2.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/skill.json` & `neon-skill-ip_address-1.2.1a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a2/test/test_skill.py` & `neon-skill-ip_address-1.2.1a3/test/test_skill.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import pytest
 
 from mock import Mock
-from mycroft_bus_client import Message
+from ovos_bus_client.message import Message
 
 from neon_minerva.tests.skill_unit_test_base import SkillTestCase
 
 
 class TestSkillMethods(SkillTestCase):
     def test_00_skill_init(self):
         # Test any parameters expected to be set in init or initialize methods
```

### Comparing `neon-skill-ip_address-1.2.1a2/version.py` & `neon-skill-ip_address-1.2.1a3/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.2.1a2"
+__version__ = "1.2.1a3"
```

