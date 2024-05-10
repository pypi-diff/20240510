# Comparing `tmp/ark-7.1.0.tar.gz` & `tmp/ark-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-7.1.0.tar", last modified: Sun Apr 30 12:00:28 2023, max compression
+gzip compressed data, was "ark-7.2.0.tar", last modified: Sun Oct 29 17:45:07 2023, max compression
```

## Comparing `ark-7.1.0.tar` & `ark-7.2.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.819955 ark-7.1.0/
--rw-r--r--   0 dmulholl   (501) staff       (20)       96 2023-04-30 12:00:28.000000 ark-7.1.0/MANIFEST.in
--rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-30 12:00:28.819335 ark-7.1.0/PKG-INFO
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.779084 ark-7.1.0/ark/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1798 2023-04-30 11:32:33.000000 ark-7.1.0/ark/__init__.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      630 2023-04-29 12:10:51.000000 ark-7.1.0/ark/__main__.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.781816 ark-7.1.0/ark/bundle/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.782575 ark-7.1.0/ark/bundle/inc/
--rw-r--r--   0 dmulholl   (501) staff       (20)      162 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/inc/menu.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.771254 ark-7.1.0/ark/bundle/lib/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.783903 ark-7.1.0/ark/bundle/lib/debug/
--rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      217 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/readme.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.784945 ark-7.1.0/ark/bundle/lib/debug/resources/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1760 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/resources/debug.css
--rw-r--r--   0 dmulholl   (501) staff       (20)     4840 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/resources/pygments.css
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.785791 ark-7.1.0/ark/bundle/lib/debug/templates/
--rw-r--r--   0 dmulholl   (501) staff       (20)     2486 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/templates/node.ibis
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.786962 ark-7.1.0/ark/bundle/lib/graphite/
--rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     1245 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/readme.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.771439 ark-7.1.0/ark/bundle/lib/graphite/resources/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.788891 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.802458 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    93768 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    13172 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    75680 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14196 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    99800 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14648 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)   189596 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    13612 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    77596 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14200 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    75580 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14388 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)     4512 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     2047 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts.css
--rw-r--r--   0 dmulholl   (501) staff       (20)    11077 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/graphite.css
--rw-r--r--   0 dmulholl   (501) staff       (20)     5027 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/pygments.css
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.802940 ark-7.1.0/ark/bundle/lib/graphite/templates/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1800 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/templates/node.ibis
--rw-r--r--   0 dmulholl   (501) staff       (20)      448 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/site.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.804494 ark-7.1.0/ark/bundle/src/
--rw-r--r--   0 dmulholl   (501) staff       (20)      551 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/about.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     4349 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/index.stx
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.805345 ark-7.1.0/ark/bundle/src/parent/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent/child-one.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent/child-two.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     1097 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.810592 ark-7.1.0/ark/cli/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1831 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/__init__.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2704 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/add.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     3091 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/build.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      903 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/clear.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1375 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/deploy.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1244 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/init.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1313 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/open.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2904 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/serve.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2319 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/tree.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     4019 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/watch.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2882 2023-04-29 12:10:51.000000 ark-7.1.0/ark/events.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.813867 ark-7.1.0/ark/extensions/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.818509 ark-7.1.0/ark/extensions/__pycache__/
--rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     3038 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_automenu.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      484 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_ibis.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      731 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_jinja.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      368 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_markdown.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1057 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_shortcodes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      335 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_syntext.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      541 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_yaml.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1658 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     3051 2023-04-29 12:10:51.000000 ark-7.1.0/ark/filters.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2604 2023-04-29 12:10:51.000000 ark-7.1.0/ark/hashes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)    11019 2023-04-29 12:10:51.000000 ark-7.1.0/ark/nodes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1880 2023-04-29 12:10:51.000000 ark-7.1.0/ark/renderers.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     7623 2023-04-29 12:10:51.000000 ark-7.1.0/ark/site.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2606 2023-04-29 12:10:51.000000 ark-7.1.0/ark/templates.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     6549 2023-04-29 12:10:51.000000 ark-7.1.0/ark/utils.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.781495 ark-7.1.0/ark.egg-info/
--rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/PKG-INFO
--rw-r--r--   0 dmulholl   (501) staff       (20)     2711 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/SOURCES.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/dependency_links.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)       33 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/entry_points.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      118 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/requires.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        4 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/top_level.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     1212 2016-08-25 13:09:14.000000 ark-7.1.0/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      208 2023-04-29 12:10:51.000000 ark-7.1.0/readme.md
--rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-04-30 12:00:28.820130 ark-7.1.0/setup.cfg
--rwxr-xr-x   0 dmulholl   (501) staff       (20)     2084 2023-04-30 11:29:49.000000 ark-7.1.0/setup.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.206774 ark-7.2.0/
+-rw-r--r--   0 dmulholl   (501) staff       (20)       96 2023-10-29 17:45:07.000000 ark-7.2.0/MANIFEST.in
+-rw-r--r--   0 dmulholl   (501) staff       (20)      920 2023-10-29 17:45:07.206179 ark-7.2.0/PKG-INFO
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.173939 ark-7.2.0/ark/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1798 2023-10-29 15:12:19.000000 ark-7.2.0/ark/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      630 2023-04-29 12:10:51.000000 ark-7.2.0/ark/__main__.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.177224 ark-7.2.0/ark/bundle/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6148 2023-10-29 15:07:44.000000 ark-7.2.0/ark/bundle/.DS_Store
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.177821 ark-7.2.0/ark/bundle/inc/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      162 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/inc/menu.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.178312 ark-7.2.0/ark/bundle/lib/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6148 2023-10-29 15:07:49.000000 ark-7.2.0/ark/bundle/lib/.DS_Store
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.179321 ark-7.2.0/ark/bundle/lib/debug/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/lib/debug/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      217 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/lib/debug/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.180238 ark-7.2.0/ark/bundle/lib/debug/resources/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1760 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/lib/debug/resources/debug.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4840 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/lib/debug/resources/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.180769 ark-7.2.0/ark/bundle/lib/debug/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2486 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/lib/debug/templates/node.ibis
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.181745 ark-7.2.0/ark/bundle/lib/graphite/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1804 2023-10-29 17:12:18.000000 ark-7.2.0/ark/bundle/lib/graphite/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.165902 ark-7.2.0/ark/bundle/lib/graphite/resources/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.184173 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      929 2023-10-21 20:21:19.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/code.js
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.192088 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    93768 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13172 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75680 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14196 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    99800 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14648 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)   189596 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13612 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    77596 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14200 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75580 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14388 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     4512 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2047 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11508 2023-10-15 20:47:42.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/graphite.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     5027 2023-04-30 12:01:24.000000 ark-7.2.0/ark/bundle/lib/graphite/resources/assets/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.192689 ark-7.2.0/ark/bundle/lib/graphite/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1938 2023-10-29 17:26:10.000000 ark-7.2.0/ark/bundle/lib/graphite/templates/node.ibis
+-rw-r--r--   0 dmulholl   (501) staff       (20)      448 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/site.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.194245 ark-7.2.0/ark/bundle/src/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      551 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/src/about.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4349 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/src/index.stx
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.195348 ark-7.2.0/ark/bundle/src/parent/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/src/parent/child-one.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/src/parent/child-two.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1097 2023-04-29 12:10:51.000000 ark-7.2.0/ark/bundle/src/parent.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.199176 ark-7.2.0/ark/cli/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1831 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2704 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/add.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3091 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/build.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      903 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/clear.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1375 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/deploy.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1244 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/init.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1313 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/open.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2904 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/serve.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2319 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/tree.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4019 2023-04-29 12:10:51.000000 ark-7.2.0/ark/cli/watch.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2882 2023-04-29 12:10:51.000000 ark-7.2.0/ark/events.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.202217 ark-7.2.0/ark/extensions/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.205566 ark-7.2.0/ark/extensions/__pycache__/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3240 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_automenu.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1198 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_ibis.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1490 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_jinja.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      873 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_markdown.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1617 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_shortcodes.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      785 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_syntext.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1167 2023-10-29 16:56:25.000000 ark-7.2.0/ark/extensions/__pycache__/ark_yaml.cpython-312.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3038 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_automenu.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      484 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_ibis.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      731 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_jinja.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      368 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_markdown.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1057 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_shortcodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      335 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_syntext.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      541 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions/ark_yaml.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1658 2023-04-29 12:10:51.000000 ark-7.2.0/ark/extensions.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3051 2023-04-29 12:10:51.000000 ark-7.2.0/ark/filters.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2604 2023-04-29 12:10:51.000000 ark-7.2.0/ark/hashes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11019 2023-04-29 12:10:51.000000 ark-7.2.0/ark/nodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1880 2023-04-29 12:10:51.000000 ark-7.2.0/ark/renderers.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     7623 2023-04-29 12:10:51.000000 ark-7.2.0/ark/site.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2606 2023-04-29 12:10:51.000000 ark-7.2.0/ark/templates.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6549 2023-04-29 12:10:51.000000 ark-7.2.0/ark/utils.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-29 17:45:07.175977 ark-7.2.0/ark.egg-info/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      920 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/PKG-INFO
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2806 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/SOURCES.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/dependency_links.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       33 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/entry_points.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      118 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/requires.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        4 2023-10-29 17:45:07.000000 ark-7.2.0/ark.egg-info/top_level.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1212 2016-08-25 13:09:14.000000 ark-7.2.0/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      210 2023-05-24 16:27:37.000000 ark-7.2.0/readme.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-10-29 17:45:07.206920 ark-7.2.0/setup.cfg
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     2084 2023-04-30 11:29:49.000000 ark-7.2.0/setup.py
```

### Comparing `ark-7.1.0/PKG-INFO` & `ark-7.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: ark
-Version: 7.1.0
+Version: 7.2.0
 Summary: A static website generator for people who enjoy the simpler things in life.
 Home-page: https://github.com/dmulholl/ark
 Author: Darren Mulholland
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Public Domain
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.8
+Requires-Dist: markdown~=3.0
+Requires-Dist: pygments~=2.0
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: jinja2~=3.0
+Requires-Dist: syntext~=3.0
+Requires-Dist: ibis~=3.0
+Requires-Dist: shortcodes~=5.1
+Requires-Dist: argslib~=2.0
+Requires-Dist: colorama~=0.4
 
 
 A static website generator for people who enjoy the simpler things in life.
 
 * `Github <https://github.com/dmulholl/ark>`_
 * `Documentation <http://www.dmulholl.com/docs/ark/main/>`_
 * `Demo <http://www.dmulholl.com/demos/ark/>`_
```

### Comparing `ark-7.1.0/ark/__init__.py` & `ark-7.2.0/ark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ------------------------------------------------------------------------------
 # Ark: a static website generator.
 # ------------------------------------------------------------------------------
 
-__version__ = '7.1.0'
+__version__ = '7.2.0'
 
 import sys
 if sys.version_info < (3, 10):
     sys.exit('Error: Ark requires Python 3.10 or later.')
 
 
 # On Windows, use the 'colorama' package if it's available to support ANSI
```

### Comparing `ark-7.1.0/ark/__main__.py` & `ark-7.2.0/ark/__main__.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/debug/license.txt` & `ark-7.2.0/ark/bundle/lib/debug/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/debug/resources/debug.css` & `ark-7.2.0/ark/bundle/lib/debug/resources/debug.css`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/debug/resources/pygments.css` & `ark-7.2.0/ark/bundle/lib/debug/resources/pygments.css`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/debug/templates/node.ibis` & `ark-7.2.0/ark/bundle/lib/debug/templates/node.ibis`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/license.txt` & `ark-7.2.0/ark/bundle/lib/graphite/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts.css` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/fonts.css`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/graphite.css` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/graphite.css`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,36 @@
     margin: 0 2px;
     padding: 1px 5px;
     border: 1px solid #e8e8e8;
     border-radius: 3px;
     background-color: #f8f8f8;
 }
 
+.pre-copy-wrapper {
+    position: relative;
+}
+
+.pre-copy-wrapper button {
+    padding: 6px;
+    background: transparent;
+    border: none;
+    position: absolute;
+    top: 10px;
+    right: 10px;
+    opacity: 0.3;
+    cursor: pointer;
+    color: black;
+    font-size: 12px;
+    font-family: Consolas, monospace;
+}
+
+.pre-copy-wrapper button:hover {
+    opacity: 0.5;
+}
+
 /**
  * Lists
  */
 
 ul, ol {
     margin: 35px 0;
     padding: 0 0 0 20px;
@@ -703,14 +725,18 @@
         font-size: 24px;
     }
 
     pre, code {
         font-size: 12px;
     }
 
+    .pre-copy-wrapper button {
+        font-size: 11px;
+    }
+
     .small {
         font-size: 15px;
     }
 
     .main .title .subtitle {
         width: auto;
     }
```

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/pygments.css` & `ark-7.2.0/ark/bundle/lib/graphite/resources/assets/pygments.css`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/lib/graphite/templates/node.ibis` & `ark-7.2.0/ark/bundle/lib/graphite/templates/node.ibis`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <title>{{ node.meta_title || node.title || site.title }}</title>
+
+        {% if node.meta_description %}
+            <meta name="description" content="{$ node.meta_description.strip() $}">
+        {% endif %}
+
         <link rel="stylesheet" href="@root/assets/fonts.css">
         <link rel="stylesheet" href="@root/assets/graphite.css">
         <link rel="stylesheet" href="@root/assets/pygments.css">
-        {% if node.meta_description %}
-            <meta name="description" content="{$ node.meta_description.strip() $}">
+
+        {% if not site.graphite.disable_copy_button %}
+            <script src="@root/assets/code.js"></script>
         {% endif %}
+
         {{ inc.head }}
     </head>
     <body class="{$ classes|join(' ') $}">
         <header class="masthead">
             <h1><a href="@root/">{{ site.title || "Site Title" }}</a></h1>
             {% if site.tagline %}
                 <p class="tagline">{{ site.tagline.strip() }}</p>
@@ -27,20 +34,22 @@
                     <span class="icon close-icon">✕</span>
                     <span class="icon open-icon">☰</span>
                     <span class="text">Menu</span>
                 </label>
                 {{ inc.menu || automenu }}
             </nav>
         </header>
+
         <article class="main">
             <header class="title">
                 <h1>{{ node.title }}</h1>
                 {% if node.subtitle %}
                     <p class="subtitle">{{ node.subtitle }}</p>
                 {% endif %}
                 <hr>
             </header>
             {{ node.html }}
         </article>
+
         {{ inc.foot }}
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 {% if node.meta_description %}
+{% endif %}
+{% if not site.graphite.disable_copy_button %}
 {% endif %} {{ inc.head }}
 ************ _{{_{{_ _ss_ii_tt_ee_.._tt_ii_tt_ll_ee_ _||_||_ _""_SS_ii_tt_ee_ _TT_ii_tt_ll_ee_""_ _}}_}} ************
 {% if site.tagline %}
 {{ site.tagline.strip() }}
 {% endif %} {% if site.version %}
 {{ site.version.strip() }}
 {% endif %} ??✕ ☰ Menu {{ inc.menu || automenu }}
```

### Comparing `ark-7.1.0/ark/bundle/src/about.md` & `ark-7.2.0/ark/bundle/src/about.md`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/src/index.stx` & `ark-7.2.0/ark/bundle/src/index.stx`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/src/parent/child-one.md` & `ark-7.2.0/ark/bundle/src/parent/child-one.md`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/src/parent/child-two.md` & `ark-7.2.0/ark/bundle/src/parent/child-two.md`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/bundle/src/parent.md` & `ark-7.2.0/ark/bundle/src/parent.md`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/__init__.py` & `ark-7.2.0/ark/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/add.py` & `ark-7.2.0/ark/cli/add.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/build.py` & `ark-7.2.0/ark/cli/build.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/clear.py` & `ark-7.2.0/ark/cli/clear.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/deploy.py` & `ark-7.2.0/ark/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/init.py` & `ark-7.2.0/ark/cli/init.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/open.py` & `ark-7.2.0/ark/cli/open.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/serve.py` & `ark-7.2.0/ark/cli/serve.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/tree.py` & `ark-7.2.0/ark/cli/tree.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/cli/watch.py` & `ark-7.2.0/ark/cli/watch.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/events.py` & `ark-7.2.0/ark/events.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc` & `ark-7.2.0/ark/extensions/__pycache__/ark_jinja.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Sat Apr 29 12:10:51 2023 UTC, .py size: 731 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,94 @@
-00000000: a70d 0d0a 0000 0000 4b09 4d64 db02 0000  ........K.Md....
+00000000: cb0d 0d0a 0000 0000 4b09 4d64 db02 0000  ........K.Md....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 ea00 0000 9700 6400 6401  ............d.d.
-00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6e0d  l.Z...d.d.l.Z.n.
-00000040: 2300 6502 2400 7205 0100 6401 5a01 5900  #.e.$.r...d.Z.Y.
-00000050: 6e04 7700 7803 5900 7701 6401 6103 6501  n.w.x.Y.w.d.a.e.
-00000060: 7257 6500 6a04 0000 0000 0000 0000 a005  rWe.j...........
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 6500 6a04 0000 0000 0000 0000  ....e.j.........
-00000090: 6a06 0000 0000 0000 0000 6a07 0000 0000  j.........j.....
-000000a0: 0000 0000 a601 0000 ab01 0000 0000 0000  ................
-000000b0: 0000 6402 8400 a600 0000 ab00 0000 0000  ..d.............
-000000c0: 0000 0000 5a08 6500 6a09 0000 0000 0000  ....Z.e.j.......
-000000d0: 0000 a005 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0000 0000 0000 0000 6403 a601 0000 ab01  ........d.......
-000000f0: 0000 0000 0000 0000 6404 8400 a600 0000  ........d.......
-00000100: ab00 0000 0000 0000 0000 5a0a 6401 5300  ..........Z.d.S.
-00000110: 6401 5300 2905 e900 0000 004e 6300 0000  d.S.)......Nc...
-00000120: 0000 0000 0000 0000 0006 0000 0003 0000  ................
-00000130: 00f3 fe00 0000 9700 6401 7401 0000 0000  ........d.t.....
-00000140: 0000 0000 0000 6a01 0000 0000 0000 0000  ......j.........
-00000150: 7404 0000 0000 0000 0000 0000 6a03 0000  t...........j...
-00000160: 0000 0000 0000 a004 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 6402 a601  ............d...
-00000180: 0000 ab01 0000 0000 0000 0000 a601 0000  ................
-00000190: ab01 0000 0000 0000 0000 6901 7d00 7c00  ..........i.}.|.
-000001a0: a005 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 7404 0000 0000 0000 0000  ......t.........
-000001c0: 0000 6a03 0000 0000 0000 0000 6a06 0000  ..j.........j...
-000001d0: 0000 0000 0000 a007 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 6403 6900  ............d.i.
-000001f0: a602 0000 ab02 0000 0000 0000 0000 a601  ................
-00000200: 0000 ab01 0000 0000 0000 0000 0100 7401  ..............t.
-00000210: 0000 0000 0000 0000 0000 6a08 0000 0000  ..........j.....
-00000220: 0000 0000 6404 6900 7c00 a401 8e01 6109  ....d.i.|.....a.
-00000230: 6400 5300 2905 4eda 066c 6f61 6465 72da  d.S.).N..loader.
-00000240: 0974 656d 706c 6174 6573 da0e 6a69 6e6a  .templates..jinj
-00000250: 615f 7365 7474 696e 6773 a900 290a da06  a_settings..)...
-00000260: 6a69 6e6a 6132 da10 4669 6c65 5379 7374  jinja2..FileSyst
-00000270: 656d 4c6f 6164 6572 da03 6172 6bda 0473  emLoader..ark..s
-00000280: 6974 65da 0574 6865 6d65 da06 7570 6461  ite..theme..upda
-00000290: 7465 da06 636f 6e66 6967 da03 6765 74da  te..config..get.
-000002a0: 0b45 6e76 6972 6f6e 6d65 6e74 da11 6a69  .Environment..ji
-000002b0: 6e6a 615f 656e 7669 726f 6e6d 656e 7429  nja_environment)
-000002c0: 01da 0873 6574 7469 6e67 7373 0100 0000  ...settingss....
-000002d0: 20fa 372f 5573 6572 732f 646d 756c 686f   .7/Users/dmulho
-000002e0: 6c6c 2f64 6576 2f73 7263 2f61 726b 2f61  ll/dev/src/ark/a
-000002f0: 726b 2f65 7874 656e 7369 6f6e 732f 6172  rk/extensions/ar
-00000300: 6b5f 6a69 6e6a 612e 7079 da1c 696e 6974  k_jinja.py..init
-00000310: 6961 6c69 7a65 5f6a 696e 6a61 5f65 6e76  ialize_jinja_env
-00000320: 6972 6f6e 6d65 6e74 7214 0000 000d 0000  ironmentr.......
-00000330: 0073 6f00 0000 8000 f006 000d 1595 66d4  .so...........f.
-00000340: 162d ad63 ac68 af6e aa6e b85b d12e 49d4  .-.c.h.n.n.[..I.
-00000350: 2e49 d116 4ad4 164a f003 0214 0a88 08f0  .I..J..J........
-00000360: 0600 0911 8f0f 8a0f 9d03 9c08 9c0f d718  ................
-00000370: 2bd2 182b d02c 3cb8 62d1 1841 d418 41d1  +..+.,<.b..A..A.
-00000380: 0842 d408 42d0 0842 e51c 22d4 1c2e d01c  .B..B..B..".....
-00000390: 3ad0 1c3a b018 d01c 3ad0 1c3a d008 19d0  :..:....:..:....
-000003a0: 0819 d008 19f3 0000 0000 da05 6a69 6e6a  ............jinj
-000003b0: 6163 0200 0000 0000 0000 0000 0000 0300  ac..............
-000003c0: 0000 0300 0000 f360 0000 0097 0074 0000  .......`.....t..
-000003d0: 0000 0000 0000 0000 00a0 0100 0000 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-000003f0: 01a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-00000400: 027c 02a0 0200 0000 0000 0000 0000 0000  .|..............
-00000410: 0000 0000 0000 0000 007c 00a6 0100 00ab  .........|......
-00000420: 0100 0000 0000 0000 0053 0029 014e 2903  .........S.).N).
-00000430: 7211 0000 00da 0c67 6574 5f74 656d 706c  r......get_templ
-00000440: 6174 65da 0672 656e 6465 7229 03da 0970  ate..render)...p
-00000450: 6167 655f 6461 7461 da11 7465 6d70 6c61  age_data..templa
-00000460: 7465 5f66 696c 656e 616d 65da 0874 656d  te_filename..tem
-00000470: 706c 6174 6573 0300 0000 2020 2072 1300  plates....   r..
-00000480: 0000 da0b 7265 6e64 6572 5f70 6167 6572  ....render_pager
-00000490: 1d00 0000 1600 0000 7328 0000 0080 00e5  ........s(......
-000004a0: 1324 d713 31d2 1331 d032 43d1 1344 d413  .$..1..1.2C..D..
-000004b0: 4488 08d8 0f17 8f7f 8a7f 9879 d10f 29d4  D..........y..).
-000004c0: 0f29 d008 2972 1500 0000 290b 720a 0000  .)..)r....).r...
-000004d0: 0072 0800 0000 da0b 496d 706f 7274 4572  .r......ImportEr
-000004e0: 726f 7272 1100 0000 da06 6576 656e 7473  rorr......events
-000004f0: da08 7265 6769 7374 6572 da05 4576 656e  ..register..Even
-00000500: 74da 0449 4e49 5472 1400 0000 7205 0000  t..INITr....r...
-00000510: 0072 1d00 0000 7207 0000 0072 1500 0000  .r....r....r....
-00000520: 7213 0000 00fa 083c 6d6f 6475 6c65 3e72  r......<module>r
-00000530: 2300 0000 0100 0000 73c6 0000 00f0 0301  #.......s.......
-00000540: 0101 f006 0001 0b80 0a80 0a80 0af0 0403  ................
-00000550: 0112 d804 1180 4d80 4d80 4d80 4df8 d807  ......M.M.M.M...
-00000560: 12f0 0001 0112 f000 0101 12f0 0001 0112  ................
-00000570: d80d 1180 4680 4680 46f0 0301 0112 f8f8  ....F.F.F.......
-00000580: f8f0 0600 1519 d000 11e0 0309 f000 0d01  ................
-00000590: 2ad8 0508 845a d705 18d2 0518 9813 9c1a  *....Z..........
-000005a0: d419 29d4 192e d105 2fd4 052f f002 0605  ..)...../../....
-000005b0: 3bf0 0006 053b f103 0006 30d4 052f f002  ;....;....0../..
-000005c0: 0605 3bf0 1000 0609 845d d705 1bd2 051b  ..;......]......
-000005d0: 9847 d105 24d4 0524 f002 0205 2af0 0002  .G..$..$....*...
-000005e0: 052a f103 0006 25d4 0524 f002 0205 2af0  .*....%..$....*.
-000005f0: 0002 052a f000 0205 2af0 170d 012a f000  ...*....*....*..
-00000600: 0d01 2a73 0c00 0000 8604 0b00 8b07 1503  ..*s............
-00000610: 9401 1503                                ....
+00000020: 0000 0000 00f3 fa00 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6401  l.Z...d.d.l.Z.d.
+00000040: 6103 6501 7261 6500 6a08 0000 0000 0000  a.e.rae.j.......
+00000050: 0000 0000 0000 0000 0000 0000 6a0b 0000  ............j...
+00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000070: 6500 6a08 0000 0000 0000 0000 0000 0000  e.j.............
+00000080: 0000 0000 0000 6a0c 0000 0000 0000 0000  ......j.........
+00000090: 0000 0000 0000 0000 0000 6a0e 0000 0000  ..........j.....
+000000a0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
+000000b0: 0000 0000 0000 6402 8400 ab00 0000 0000  ......d.........
+000000c0: 0000 5a08 6500 6a12 0000 0000 0000 0000  ..Z.e.j.........
+000000d0: 0000 0000 0000 0000 0000 6a0b 0000 0000  ..........j.....
+000000e0: 0000 0000 0000 0000 0000 0000 0000 6403  ..............d.
+000000f0: ab01 0000 0000 0000 6404 8400 ab00 0000  ........d.......
+00000100: 0000 0000 5a0a 7901 7901 2300 6502 2400  ....Z.y.y.#.e.$.
+00000110: 7205 0100 6401 5a01 5900 8c6f 7700 7803  r...d.Z.Y..ow.x.
+00000120: 5900 7701 2905 e900 0000 004e 6300 0000  Y.w.)......Nc...
+00000130: 0000 0000 0000 0000 0006 0000 0003 0000  ................
+00000140: 00f3 0801 0000 9700 6401 7401 0000 0000  ........d.t.....
+00000150: 0000 0000 6a02 0000 0000 0000 0000 0000  ....j...........
+00000160: 0000 0000 0000 0000 7404 0000 0000 0000  ........t.......
+00000170: 0000 6a06 0000 0000 0000 0000 0000 0000  ..j.............
+00000180: 0000 0000 0000 6a09 0000 0000 0000 0000  ......j.........
+00000190: 0000 0000 0000 0000 0000 6402 ab01 0000  ..........d.....
+000001a0: 0000 0000 ab01 0000 0000 0000 6901 7d00  ............i.}.
+000001b0: 7c00 6a0b 0000 0000 0000 0000 0000 0000  |.j.............
+000001c0: 0000 0000 0000 7404 0000 0000 0000 0000  ......t.........
+000001d0: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+000001e0: 0000 0000 6a0c 0000 0000 0000 0000 0000  ....j...........
+000001f0: 0000 0000 0000 0000 6a0f 0000 0000 0000  ........j.......
+00000200: 0000 0000 0000 0000 0000 0000 6403 6900  ............d.i.
+00000210: ab02 0000 0000 0000 ab01 0000 0000 0000  ................
+00000220: 0100 7401 0000 0000 0000 0000 6a10 0000  ..t.........j...
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 6404 6900 7c00 a401 8e01 6109 7900 2905  d.i.|.....a.y.).
+00000250: 4eda 066c 6f61 6465 72da 0974 656d 706c  N..loader..templ
+00000260: 6174 6573 da0e 6a69 6e6a 615f 7365 7474  ates..jinja_sett
+00000270: 696e 6773 a900 290a da06 6a69 6e6a 6132  ings..)...jinja2
+00000280: da10 4669 6c65 5379 7374 656d 4c6f 6164  ..FileSystemLoad
+00000290: 6572 da03 6172 6bda 0473 6974 65da 0574  er..ark..site..t
+000002a0: 6865 6d65 da06 7570 6461 7465 da06 636f  heme..update..co
+000002b0: 6e66 6967 da03 6765 74da 0b45 6e76 6972  nfig..get..Envir
+000002c0: 6f6e 6d65 6e74 da11 6a69 6e6a 615f 656e  onment..jinja_en
+000002d0: 7669 726f 6e6d 656e 7429 01da 0873 6574  vironment)...set
+000002e0: 7469 6e67 7373 0100 0000 20fa 372f 5573  tingss.... .7/Us
+000002f0: 6572 732f 646d 756c 686f 6c6c 2f64 6576  ers/dmulholl/dev
+00000300: 2f73 7263 2f61 726b 2f61 726b 2f65 7874  /src/ark/ark/ext
+00000310: 656e 7369 6f6e 732f 6172 6b5f 6a69 6e6a  ensions/ark_jinj
+00000320: 612e 7079 da1c 696e 6974 6961 6c69 7a65  a.py..initialize
+00000330: 5f6a 696e 6a61 5f65 6e76 6972 6f6e 6d65  _jinja_environme
+00000340: 6e74 7214 0000 000d 0000 0073 6000 0000  ntr........s`...
+00000350: 8000 f006 000d 1594 66d7 162d d116 2dac  ........f..-..-.
+00000360: 63af 68a9 68af 6ea9 6eb8 5bd3 2e49 d316  c.h.h.n.n.[..I..
+00000370: 4af0 0302 140a 8808 f006 0009 118f 0f89  J...............
+00000380: 0f9c 039f 0899 089f 0f99 0fd7 182b d118  .............+..
+00000390: 2bd0 2c3c b862 d318 41d4 0842 e41c 22d7  +.,<.b..A..B..".
+000003a0: 1c2e d11c 2ed1 1c3a b018 d11c 3ad1 0819  .......:....:...
+000003b0: f300 0000 00da 056a 696e 6a61 6302 0000  .......jinjac...
+000003c0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000003d0: 00f3 4e00 0000 9700 7400 0000 0000 0000  ..N.....t.......
+000003e0: 0000 6a03 0000 0000 0000 0000 0000 0000  ..j.............
+000003f0: 0000 0000 0000 7c01 ab01 0000 0000 0000  ......|.........
+00000400: 7d02 7c02 6a05 0000 0000 0000 0000 0000  }.|.j...........
+00000410: 0000 0000 0000 0000 7c00 ab01 0000 0000  ........|.......
+00000420: 0000 5300 2901 4e29 0372 1100 0000 da0c  ..S.).N).r......
+00000430: 6765 745f 7465 6d70 6c61 7465 da06 7265  get_template..re
+00000440: 6e64 6572 2903 da09 7061 6765 5f64 6174  nder)...page_dat
+00000450: 61da 1174 656d 706c 6174 655f 6669 6c65  a..template_file
+00000460: 6e61 6d65 da08 7465 6d70 6c61 7465 7303  name..templates.
+00000470: 0000 0020 2020 7213 0000 00da 0b72 656e  ...   r......ren
+00000480: 6465 725f 7061 6765 721d 0000 0016 0000  der_pager.......
+00000490: 0073 2200 0000 8000 e413 24d7 1331 d113  .s".......$..1..
+000004a0: 31d0 3243 d313 4488 08d8 0f17 8f7f 897f  1.2C..D.........
+000004b0: 9879 d30f 29d0 0829 7215 0000 0029 0b72  .y..)..)r....).r
+000004c0: 0a00 0000 7208 0000 00da 0b49 6d70 6f72  ....r......Impor
+000004d0: 7445 7272 6f72 7211 0000 00da 0665 7665  tErrorr......eve
+000004e0: 6e74 73da 0872 6567 6973 7465 72da 0545  nts..register..E
+000004f0: 7665 6e74 da04 494e 4954 7214 0000 0072  vent..INITr....r
+00000500: 0500 0000 721d 0000 0072 0700 0000 7215  ....r....r....r.
+00000510: 0000 0072 1300 0000 fa08 3c6d 6f64 756c  ...r......<modul
+00000520: 653e 7223 0000 0001 0000 0073 8c00 0000  e>r#.......s....
+00000530: f003 0101 01f3 0600 010b f004 0301 12db  ................
+00000540: 0411 f008 0015 19d0 0011 e103 09d8 0508  ................
+00000550: 875a 815a d705 18d1 0518 9813 9f1a 991a  .Z.Z............
+00000560: d719 29d1 1929 d719 2ed1 192e d305 2ff1  ..)..)......../.
+00000570: 0206 053b f303 0006 30f0 0206 053b f010  ...;....0....;..
+00000580: 0006 0987 5d81 5dd7 051b d105 1b98 47d3  ....].].......G.
+00000590: 0524 f102 0205 2af3 0300 0625 f102 0205  .$....*....%....
+000005a0: 2af0 1700 040a f8f0 0b00 0813 f200 0101  *...............
+000005b0: 12d8 0d11 8246 f003 0101 12fa 7311 0000  .....F......s...
+000005c0: 0086 0441 3000 c130 0741 3a03 c139 0141  ...A0..0.A:..9.A
+000005d0: 3a03                                     :.
```

### Comparing `ark-7.1.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc` & `ark-7.2.0/ark/extensions/__pycache__/ark_markdown.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Sat Apr 29 12:10:51 2023 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,55 @@
-00000000: a70d 0d0a 0000 0000 4b09 4d64 7001 0000  ........K.Mdp...
+00000000: cb0d 0d0a 0000 0000 4b09 4d64 7001 0000  ........K.Mdp...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 de00 0000 9700 6400 6401  ............d.d.
-00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6e0d  l.Z...d.d.l.Z.n.
-00000040: 2300 6502 2400 7205 0100 6401 5a01 5900  #.e.$.r...d.Z.Y.
-00000050: 6e04 7700 7803 5900 7701 6501 7253 6500  n.w.x.Y.w.e.rSe.
-00000060: 6a03 0000 0000 0000 0000 6a04 0000 0000  j.........j.....
-00000070: 0000 0000 a005 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 6402 a601 0000  ..........d.....
-00000090: ab01 0000 0000 0000 0000 7001 6900 5a06  ..........p.i.Z.
-000000a0: 0200 6501 6a07 0000 0000 0000 0000 6405  ..e.j.........d.
-000000b0: 6900 6506 a401 8e01 5a08 6500 6a09 0000  i.e.....Z.e.j...
-000000c0: 0000 0000 0000 a00a 0000 0000 0000 0000  ................
-000000d0: 0000 0000 0000 0000 0000 0000 6403 a601  ............d...
-000000e0: 0000 ab01 0000 0000 0000 0000 6404 8400  ............d...
-000000f0: a600 0000 ab00 0000 0000 0000 0000 5a0b  ..............Z.
-00000100: 6401 5300 6401 5300 2906 e900 0000 004e  d.S.d.S.)......N
-00000110: da11 6d61 726b 646f 776e 5f73 6574 7469  ..markdown_setti
-00000120: 6e67 73da 026d 6463 0100 0000 0000 0000  ngs..mdc........
-00000130: 0000 0000 0300 0000 0300 0000 f35a 0000  .............Z..
-00000140: 0097 0074 0000 0000 0000 0000 0000 00a0  ...t............
-00000150: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 00a6 0000 00ab 0000 0000 0000  ................
-00000170: 0000 00a0 0200 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 007c 00a6 0100 00ab  .........|......
-00000190: 0100 0000 0000 0000 0053 0029 014e 2903  .........S.).N).
-000001a0: da08 7265 6e64 6572 6572 da05 7265 7365  ..renderer..rese
-000001b0: 74da 0763 6f6e 7665 7274 2901 da04 7465  t..convert)...te
-000001c0: 7874 7301 0000 0020 fa3a 2f55 7365 7273  xts.... .:/Users
-000001d0: 2f64 6d75 6c68 6f6c 6c2f 6465 762f 7372  /dmulholl/dev/sr
-000001e0: 632f 6172 6b2f 6172 6b2f 6578 7465 6e73  c/ark/ark/extens
-000001f0: 696f 6e73 2f61 726b 5f6d 6172 6b64 6f77  ions/ark_markdow
-00000200: 6e2e 7079 da0f 7265 6e64 6572 5f6d 6172  n.py..render_mar
-00000210: 6b64 6f77 6e72 0b00 0000 0e00 0000 7320  kdownr........s 
-00000220: 0000 0080 00e5 0f17 8f7e 8a7e d10f 1fd4  .........~.~....
-00000230: 0f1f d70f 27d2 0f27 a804 d10f 2dd4 0f2d  ....'..'....-..-
-00000240: d008 2df3 0000 0000 a900 290c da03 6172  ..-.......)...ar
-00000250: 6bda 086d 6172 6b64 6f77 6eda 0b49 6d70  k..markdown..Imp
-00000260: 6f72 7445 7272 6f72 da04 7369 7465 da06  ortError..site..
-00000270: 636f 6e66 6967 da03 6765 74da 0873 6574  config..get..set
-00000280: 7469 6e67 73da 084d 6172 6b64 6f77 6e72  tings..Markdownr
-00000290: 0600 0000 da09 7265 6e64 6572 6572 73da  ......renderers.
-000002a0: 0872 6567 6973 7465 7272 0b00 0000 720d  .registerr....r.
-000002b0: 0000 0072 0c00 0000 720a 0000 00fa 083c  ...r....r......<
-000002c0: 6d6f 6475 6c65 3e72 1800 0000 0100 0000  module>r........
-000002d0: 73c1 0000 00f0 0301 0101 f006 0001 0b80  s...............
-000002e0: 0a80 0a80 0af0 0403 0114 d804 1380 4f80  ..............O.
-000002f0: 4f80 4f80 4ff8 d807 12f0 0001 0114 f000  O.O.O...........
-00000300: 0101 14f0 0001 0114 d80f 1380 4880 4880  ............H.H.
-00000310: 48f0 0301 0114 f8f8 f8f0 0600 040c f000  H...............
-00000320: 0601 2ed8 0f12 8c78 8c7f d70f 22d2 0f22  .......x....".."
-00000330: d023 36d1 0f37 d40f 37d0 0f3d b832 8048  .#6..7..7..=.2.H
-00000340: d80f 2088 78d4 0f20 d00f 2cd0 0f2c a038  .. .x.. ..,..,.8
-00000350: d00f 2cd0 0f2c 8048 e005 0884 5dd7 051b  ..,..,.H....]...
-00000360: d205 1b98 44d1 0521 d405 21f0 0201 052e  ....D..!..!.....
-00000370: f000 0105 2ef1 0300 0622 d405 21f0 0201  ........."..!...
-00000380: 052e f000 0105 2ef0 0001 052e f00b 0601  ................
-00000390: 2ef0 0006 012e 730c 0000 0086 040b 008b  ......s.........
-000003a0: 0715 0394 0115 03                        .......
+00000020: 0000 0000 00f3 ee00 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6501  l.Z...d.d.l.Z.e.
+00000040: 725d 6500 6a06 0000 0000 0000 0000 0000  r]e.j...........
+00000050: 0000 0000 0000 0000 6a08 0000 0000 0000  ........j.......
+00000060: 0000 0000 0000 0000 0000 0000 6a0b 0000  ............j...
+00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000080: 6402 ab01 0000 0000 0000 7801 7302 0100  d.........x.s...
+00000090: 6900 5a06 0200 6501 6a0e 0000 0000 0000  i.Z...e.j.......
+000000a0: 0000 0000 0000 0000 0000 0000 6405 6900  ............d.i.
+000000b0: 6506 a401 8e01 5a08 6500 6a12 0000 0000  e.....Z.e.j.....
+000000c0: 0000 0000 0000 0000 0000 0000 0000 6a15  ..............j.
+000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000e0: 0000 6403 ab01 0000 0000 0000 6404 8400  ..d.........d...
+000000f0: ab00 0000 0000 0000 5a0b 7901 7901 2300  ........Z.y.y.#.
+00000100: 6502 2400 7205 0100 6401 5a01 5900 8c69  e.$.r...d.Z.Y..i
+00000110: 7700 7803 5900 7701 2906 e900 0000 004e  w.x.Y.w.)......N
+00000120: da11 6d61 726b 646f 776e 5f73 6574 7469  ..markdown_setti
+00000130: 6e67 73da 026d 6463 0100 0000 0000 0000  ngs..mdc........
+00000140: 0000 0000 0300 0000 0300 0000 f348 0000  .............H..
+00000150: 0097 0074 0000 0000 0000 0000 006a 0300  ...t.........j..
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 00ab 0000 0000 0000 006a 0500 0000 0000  .........j......
+00000180: 0000 0000 0000 0000 0000 0000 007c 00ab  .............|..
+00000190: 0100 0000 0000 0053 0029 014e 2903 da08  .......S.).N)...
+000001a0: 7265 6e64 6572 6572 da05 7265 7365 74da  renderer..reset.
+000001b0: 0763 6f6e 7665 7274 2901 da04 7465 7874  .convert)...text
+000001c0: 7301 0000 0020 fa3a 2f55 7365 7273 2f64  s.... .:/Users/d
+000001d0: 6d75 6c68 6f6c 6c2f 6465 762f 7372 632f  mulholl/dev/src/
+000001e0: 6172 6b2f 6172 6b2f 6578 7465 6e73 696f  ark/ark/extensio
+000001f0: 6e73 2f61 726b 5f6d 6172 6b64 6f77 6e2e  ns/ark_markdown.
+00000200: 7079 da0f 7265 6e64 6572 5f6d 6172 6b64  py..render_markd
+00000210: 6f77 6e72 0b00 0000 0e00 0000 731a 0000  ownr........s...
+00000220: 0080 00e4 0f17 8f7e 897e d30f 1fd7 0f27  .......~.~.....'
+00000230: d10f 27a8 04d3 0f2d d008 2df3 0000 0000  ..'....-..-.....
+00000240: a900 290c da03 6172 6bda 086d 6172 6b64  ..)...ark..markd
+00000250: 6f77 6eda 0b49 6d70 6f72 7445 7272 6f72  own..ImportError
+00000260: da04 7369 7465 da06 636f 6e66 6967 da03  ..site..config..
+00000270: 6765 74da 0873 6574 7469 6e67 73da 084d  get..settings..M
+00000280: 6172 6b64 6f77 6e72 0600 0000 da09 7265  arkdownr......re
+00000290: 6e64 6572 6572 73da 0872 6567 6973 7465  nderers..registe
+000002a0: 7272 0b00 0000 720d 0000 0072 0c00 0000  rr....r....r....
+000002b0: 720a 0000 00fa 083c 6d6f 6475 6c65 3e72  r......<module>r
+000002c0: 1800 0000 0100 0000 7386 0000 00f0 0301  ........s.......
+000002d0: 0101 f306 0001 0bf0 0403 0114 db04 13f1  ................
+000002e0: 0800 040c d80f 128f 7889 788f 7f89 7fd7  ........x.x.....
+000002f0: 0f22 d10f 22d0 2336 d30f 37d2 0f3d b832  ."..".#6..7..=.2
+00000300: 8048 d80f 2088 78d7 0f20 d10f 20d1 0f2c  .H.. .x.. .. ..,
+00000310: a038 d10f 2c80 48e0 0508 875d 815d d705  .8..,.H....].]..
+00000320: 1bd1 051b 9844 d305 21f1 0201 052e f303  .....D..!.......
+00000330: 0006 22f1 0201 052e f00b 0004 0cf8 f007  ..".............
+00000340: 0008 13f2 0001 0114 d80f 1382 48f0 0301  ............H...
+00000350: 0114 fa73 1100 0000 8604 412a 00c1 2a07  ...s......A*..*.
+00000360: 4134 03c1 3301 4134 03                   A4..3.A4.
```

### Comparing `ark-7.1.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc` & `ark-7.2.0/ark/extensions/__pycache__/ark_syntext.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Sat Apr 29 12:10:51 2023 UTC, .py size: 335 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-00000000: a70d 0d0a 0000 0000 4b09 4d64 4f01 0000  ........K.MdO...
+00000000: cb0d 0d0a 0000 0000 4b09 4d64 4f01 0000  ........K.MdO...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 c800 0000 9700 6400 6401  ............d.d.
-00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6e0d  l.Z...d.d.l.Z.n.
-00000040: 2300 6502 2400 7205 0100 6401 5a01 5900  #.e.$.r...d.Z.Y.
-00000050: 6e04 7700 7803 5900 7701 6500 6a03 0000  n.w.x.Y.w.e.j...
-00000060: 0000 0000 0000 6a04 0000 0000 0000 0000  ......j.........
-00000070: a005 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 6402 a601 0000 ab01 0000  ......d.........
-00000090: 0000 0000 0000 7003 6403 6404 6901 5a06  ......p.d.d.i.Z.
-000000a0: 6501 7225 6500 6a07 0000 0000 0000 0000  e.r%e.j.........
-000000b0: a008 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 0000 0000 6405 a601 0000 ab01 0000  ......d.........
-000000d0: 0000 0000 0000 6406 8400 a600 0000 ab00  ......d.........
-000000e0: 0000 0000 0000 0000 5a09 6401 5300 6401  ........Z.d.S.d.
-000000f0: 5300 2907 e900 0000 004e da10 7379 6e74  S.)......N..synt
-00000100: 6578 745f 7365 7474 696e 6773 da0a 7079  ext_settings..py
-00000110: 676d 656e 7469 7a65 54da 0373 7478 6301  gmentizeT..stxc.
-00000120: 0000 0000 0000 0000 0000 0005 0000 0003  ................
-00000130: 0000 00f3 3000 0000 9700 7401 0000 0000  ....0.....t.....
-00000140: 0000 0000 0000 6a01 0000 0000 0000 0000  ......j.........
-00000150: 7c00 6601 6900 7404 0000 0000 0000 0000  |.f.i.t.........
-00000160: 0000 a401 8e01 5300 2901 4e29 03da 0773  ......S.).N)...s
-00000170: 796e 7465 7874 da06 7265 6e64 6572 da08  yntext..render..
-00000180: 7365 7474 696e 6773 2901 da04 7465 7874  settings)...text
-00000190: 7301 0000 0020 fa39 2f55 7365 7273 2f64  s.... .9/Users/d
-000001a0: 6d75 6c68 6f6c 6c2f 6465 762f 7372 632f  mulholl/dev/src/
-000001b0: 6172 6b2f 6172 6b2f 6578 7465 6e73 696f  ark/ark/extensio
-000001c0: 6e73 2f61 726b 5f73 796e 7465 7874 2e70  ns/ark_syntext.p
-000001d0: 79da 0e72 656e 6465 725f 7379 6e74 6578  y..render_syntex
-000001e0: 7472 0c00 0000 0d00 0000 731a 0000 0080  tr........s.....
-000001f0: 00e5 0f16 8c7e 9864 d00f 2fd0 0f2f a568  .....~.d../../.h
-00000200: d00f 2fd0 0f2f d008 2ff3 0000 0000 290a  ../../../.....).
-00000210: da03 6172 6b72 0700 0000 da0b 496d 706f  ..arkr......Impo
-00000220: 7274 4572 726f 72da 0473 6974 65da 0663  rtError..site..c
-00000230: 6f6e 6669 67da 0367 6574 7209 0000 00da  onfig..getr.....
-00000240: 0972 656e 6465 7265 7273 da08 7265 6769  .renderers..regi
-00000250: 7374 6572 720c 0000 00a9 0072 0d00 0000  sterr......r....
-00000260: 720b 0000 00fa 083c 6d6f 6475 6c65 3e72  r......<module>r
-00000270: 1600 0000 0100 0000 73ae 0000 00f0 0301  ........s.......
-00000280: 0101 f006 0001 0b80 0a80 0a80 0af0 0403  ................
-00000290: 0113 d804 1280 4e80 4e80 4e80 4ef8 d807  ......N.N.N.N...
-000002a0: 12f0 0001 0113 f000 0101 13f0 0001 0113  ................
-000002b0: d80e 1280 4780 4780 47f0 0301 0113 f8f8  ....G.G.G.......
-000002c0: f8f0 0600 0c0f 8c38 8c3f d70b 1ed2 0b1e  .......8.?......
-000002d0: d01f 31d1 0b32 d40b 32d0 0b4a b07c c054  ..1..2..2..J.|.T
-000002e0: d036 4a80 08e0 030a f000 0301 30d8 0508  .6J.........0...
-000002f0: 845d d705 1bd2 051b 9845 d105 22d4 0522  .].......E..".."
-00000300: f002 0105 30f0 0001 0530 f103 0006 23d4  ....0....0....#.
-00000310: 0522 f002 0105 30f0 0001 0530 f000 0105  ."....0....0....
-00000320: 30f0 0503 0130 f000 0301 3073 0c00 0000  0....0....0s....
-00000330: 8604 0b00 8b07 1503 9401 1503            ............
+00000020: 0000 0000 00f3 ce00 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 0900 6400 6401 6c01 5a01 6500  l.Z...d.d.l.Z.e.
+00000040: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+00000050: 0000 0000 6a08 0000 0000 0000 0000 0000  ....j...........
+00000060: 0000 0000 0000 0000 6a0b 0000 0000 0000  ........j.......
+00000070: 0000 0000 0000 0000 0000 0000 6402 ab01  ............d...
+00000080: 0000 0000 0000 7801 7304 0100 6403 6404  ......x.s...d.d.
+00000090: 6901 5a06 6501 7222 6500 6a0e 0000 0000  i.Z.e.r"e.j.....
+000000a0: 0000 0000 0000 0000 0000 0000 0000 6a11  ..............j.
+000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000c0: 0000 6405 ab01 0000 0000 0000 6406 8400  ..d.........d...
+000000d0: ab00 0000 0000 0000 5a09 7901 7901 2300  ........Z.y.y.#.
+000000e0: 6502 2400 7205 0100 6401 5a01 5900 8c59  e.$.r...d.Z.Y..Y
+000000f0: 7700 7803 5900 7701 2907 e900 0000 004e  w.x.Y.w.)......N
+00000100: da10 7379 6e74 6578 745f 7365 7474 696e  ..syntext_settin
+00000110: 6773 da0a 7079 676d 656e 7469 7a65 54da  gs..pygmentizeT.
+00000120: 0373 7478 6301 0000 0000 0000 0000 0000  .stxc...........
+00000130: 0005 0000 0003 0000 00f3 3600 0000 9700  ..........6.....
+00000140: 7401 0000 0000 0000 0000 6a02 0000 0000  t.........j.....
+00000150: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+00000160: 6601 6900 7404 0000 0000 0000 0000 a401  f.i.t...........
+00000170: 8e01 5300 2901 4e29 03da 0773 796e 7465  ..S.).N)...synte
+00000180: 7874 da06 7265 6e64 6572 da08 7365 7474  xt..render..sett
+00000190: 696e 6773 2901 da04 7465 7874 7301 0000  ings)...texts...
+000001a0: 0020 fa39 2f55 7365 7273 2f64 6d75 6c68  . .9/Users/dmulh
+000001b0: 6f6c 6c2f 6465 762f 7372 632f 6172 6b2f  oll/dev/src/ark/
+000001c0: 6172 6b2f 6578 7465 6e73 696f 6e73 2f61  ark/extensions/a
+000001d0: 726b 5f73 796e 7465 7874 2e70 79da 0e72  rk_syntext.py..r
+000001e0: 656e 6465 725f 7379 6e74 6578 7472 0c00  ender_syntextr..
+000001f0: 0000 0d00 0000 7316 0000 0080 00e4 0f16  ......s.........
+00000200: 8f7e 897e 9864 d10f 2fa4 68d1 0f2f d008  .~.~.d../.h../..
+00000210: 2ff3 0000 0000 290a da03 6172 6b72 0700  /.....)...arkr..
+00000220: 0000 da0b 496d 706f 7274 4572 726f 72da  ....ImportError.
+00000230: 0473 6974 65da 0663 6f6e 6669 67da 0367  .site..config..g
+00000240: 6574 7209 0000 00da 0972 656e 6465 7265  etr......rendere
+00000250: 7273 da08 7265 6769 7374 6572 720c 0000  rs..registerr...
+00000260: 00a9 0072 0d00 0000 720b 0000 00fa 083c  ...r....r......<
+00000270: 6d6f 6475 6c65 3e72 1600 0000 0100 0000  module>r........
+00000280: 7376 0000 00f0 0301 0101 f306 0001 0bf0  sv..............
+00000290: 0403 0113 db04 12f0 0800 0c0f 8f38 8938  .............8.8
+000002a0: 8f3f 893f d70b 1ed1 0b1e d01f 31d3 0b32  .?.?........1..2
+000002b0: d20b 4ab0 7cc0 54d0 364a 8008 e103 0ad8  ..J.|.T.6J......
+000002c0: 0508 875d 815d d705 1bd1 051b 9845 d305  ...].].......E..
+000002d0: 22f1 0201 0530 f303 0006 23f1 0201 0530  "....0....#....0
+000002e0: f005 0004 0bf8 f00b 0008 13f2 0001 0113  ................
+000002f0: d80e 1282 47f0 0301 0113 fa73 1100 0000  ....G......s....
+00000300: 8604 411a 00c1 1a07 4124 03c1 2301 4124  ..A.....A$..#.A$
+00000310: 03                                       .
```

### Comparing `ark-7.1.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc` & `ark-7.2.0/ark/extensions/__pycache__/ark_yaml.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Sat Apr 29 12:10:51 2023 UTC, .py size: 541 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,73 @@
-00000000: a70d 0d0a 0000 0000 4b09 4d64 1d02 0000  ........K.Md....
+00000000: cb0d 0d0a 0000 0000 4b09 4d64 1d02 0000  ........K.Md....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 a800 0000 9700 6400 6401  ............d.d.
+00000020: 0000 0000 00f3 bc00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 0900 6400  l.Z.d.d.l.Z...d.
-00000040: 6401 6c02 5a02 6e0d 2300 6503 2400 7205  d.l.Z.n.#.e.$.r.
-00000050: 0100 6401 5a02 5900 6e04 7700 7803 5900  ..d.Z.Y.n.w.x.Y.
-00000060: 7701 6502 7234 6500 6a04 0000 0000 0000  w.e.r4e.j.......
-00000070: 0000 a005 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 6500 6a04 0000 0000  ........e.j.....
-00000090: 0000 0000 6a06 0000 0000 0000 0000 6a07  ....j.........j.
-000000a0: 0000 0000 0000 0000 a601 0000 ab01 0000  ................
-000000b0: 0000 0000 0000 6402 8400 a600 0000 ab00  ......d.........
-000000c0: 0000 0000 0000 0000 5a08 6401 5300 6401  ........Z.d.S.d.
-000000d0: 5300 2903 e900 0000 004e 6302 0000 0000  S.)......Nc.....
-000000e0: 0000 0000 0000 0005 0000 0003 0000 00f3  ................
-000000f0: 5001 0000 9700 7c00 a000 0000 0000 0000  P.....|.........
-00000100: 0000 0000 0000 0000 0000 0000 0000 6401  ..............d.
-00000110: a601 0000 ab01 0000 0000 0000 0000 7290  ..............r.
-00000120: 7403 0000 0000 0000 0000 0000 6a02 0000  t...........j...
-00000130: 0000 0000 0000 6402 7c00 7402 0000 0000  ......d.|.t.....
-00000140: 0000 0000 0000 6a03 0000 0000 0000 0000  ......j.........
-00000150: a603 0000 ab03 0000 0000 0000 0000 7801  ..............x.
-00000160: 7d02 726e 7c00 7c02 a004 0000 0000 0000  }.rn|.|.........
-00000170: 0000 0000 0000 0000 0000 0000 0000 6403  ..............d.
-00000180: a601 0000 ab01 0000 0000 0000 0000 6400  ..............d.
-00000190: 8502 1900 0000 0000 0000 0000 7d00 740b  ............}.t.
-000001a0: 0000 0000 0000 0000 0000 6a06 0000 0000  ..........j.....
-000001b0: 0000 0000 7c02 a007 0000 0000 0000 0000  ....|...........
-000001c0: 0000 0000 0000 0000 0000 0000 6404 a601  ............d...
-000001d0: 0000 ab01 0000 0000 0000 0000 a601 0000  ................
-000001e0: ab01 0000 0000 0000 0000 7d03 7411 0000  ..........}.t...
-000001f0: 0000 0000 0000 0000 7c03 7412 0000 0000  ........|.t.....
-00000200: 0000 0000 0000 a602 0000 ab02 0000 0000  ................
-00000210: 0000 0000 7215 7c01 a00a 0000 0000 0000  ....r.|.........
-00000220: 0000 0000 0000 0000 0000 0000 0000 7c03  ..............|.
-00000230: a601 0000 ab01 0000 0000 0000 0000 0100  ................
-00000240: 7c00 5300 2905 4e7a 042d 2d2d 0a7a 125e  |.S.).Nz.---.z.^
-00000250: 2d2d 2d5c 6e28 2e2a 3f5c 6e29 2d2d 2d5c  ---\n(.*?\n)---\
-00000260: 6e72 0200 0000 e901 0000 0029 0bda 0a73  nr.........)...s
-00000270: 7461 7274 7377 6974 68da 0272 65da 056d  tartswith..re..m
-00000280: 6174 6368 da06 444f 5441 4c4c da03 656e  atch..DOTALL..en
-00000290: 64da 0479 616d 6cda 0973 6166 655f 6c6f  d..yaml..safe_lo
-000002a0: 6164 da05 6772 6f75 70da 0a69 7369 6e73  ad..group..isins
-000002b0: 7461 6e63 65da 0464 6963 74da 0675 7064  tance..dict..upd
-000002c0: 6174 6529 04da 0474 6578 74da 096d 6574  ate)...text..met
-000002d0: 615f 6469 6374 7207 0000 00da 0464 6174  a_dictr......dat
-000002e0: 6173 0400 0000 2020 2020 fa36 2f55 7365  as....    .6/Use
-000002f0: 7273 2f64 6d75 6c68 6f6c 6c2f 6465 762f  rs/dmulholl/dev/
-00000300: 7372 632f 6172 6b2f 6172 6b2f 6578 7465  src/ark/ark/exte
-00000310: 6e73 696f 6e73 2f61 726b 5f79 616d 6c2e  nsions/ark_yaml.
-00000320: 7079 da11 7061 7273 655f 7961 6d6c 5f68  py..parse_yaml_h
-00000330: 6561 6465 7272 1400 0000 0c00 0000 7390  eaderr........s.
-00000340: 0000 0080 00e0 0b0f 8f3f 8a3f 9837 d10b  .........?.?.7..
-00000350: 23d4 0b23 f000 0509 2bdd 181a 9c08 d021  #..#....+......!
-00000360: 36b8 04bd 62bc 69d1 1848 d418 48d0 0f48  6...b.i..H..H..H
-00000370: 8875 f000 040d 2bd8 171b 9845 9f49 9a49  .u....+....E.I.I
-00000380: a061 994c 9c4c 984d 984d d417 2a90 04dd  .a.L.L.M.M..*...
-00000390: 171b 947e a065 a76b a26b b021 a16e a46e  ...~.e.k.k.!.n.n
-000003a0: d117 35d4 1735 9004 dd13 1d98 64a5 44d1  ..5..5......d.D.
-000003b0: 1329 d413 29f0 0001 112b d814 1dd7 1424  .)..)....+.....$
-000003c0: d214 24a0 54d1 142a d414 2ad0 142a d80f  ..$.T..*..*..*..
-000003d0: 1388 0bf3 0000 0000 2909 da03 6172 6b72  ........)...arkr
-000003e0: 0600 0000 720a 0000 00da 0b49 6d70 6f72  ....r......Impor
-000003f0: 7445 7272 6f72 da07 6669 6c74 6572 73da  tError..filters.
-00000400: 0872 6567 6973 7465 72da 0646 696c 7465  .register..Filte
-00000410: 72da 0946 494c 455f 5445 5854 7214 0000  r..FILE_TEXTr...
-00000420: 00a9 0072 1500 0000 7213 0000 00fa 083c  ...r....r......<
-00000430: 6d6f 6475 6c65 3e72 1d00 0000 0100 0000  module>r........
-00000440: 739d 0000 00f0 0301 0101 f006 0001 0b80  s...............
-00000450: 0a80 0a80 0ad8 0009 8009 8009 8009 f004  ................
-00000460: 0301 10d8 040f 804b 804b 804b 804b f8d8  .......K.K.K.K..
-00000470: 0712 f000 0101 10f0 0001 0110 f000 0101  ................
-00000480: 10d8 0b0f 8044 8044 8044 f003 0101 10f8  .....D.D.D......
-00000490: f8f8 f006 0004 08f0 0009 0114 d805 0884  ................
-000004a0: 5bd7 0519 d205 1998 239c 2bd4 1a2c d41a  [.......#.+..,..
-000004b0: 36d1 0537 d405 37f0 0207 0514 f000 0705  6..7..7.........
-000004c0: 14f1 0300 0638 d405 37f0 0207 0514 f000  .....8..7.......
-000004d0: 0705 14f0 0007 0514 f005 0901 14f0 0009  ................
-000004e0: 0114 730c 0000 008a 040f 008f 0719 0398  ..s.............
-000004f0: 0119 03                                  ...
+00000040: 6401 6c02 5a02 6502 7240 6500 6a08 0000  d.l.Z.e.r@e.j...
+00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000060: 6a0b 0000 0000 0000 0000 0000 0000 0000  j...............
+00000070: 0000 0000 6500 6a08 0000 0000 0000 0000  ....e.j.........
+00000080: 0000 0000 0000 0000 0000 6a0c 0000 0000  ..........j.....
+00000090: 0000 0000 0000 0000 0000 0000 0000 6a0e  ..............j.
+000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000b0: 0000 ab01 0000 0000 0000 6402 8400 ab00  ..........d.....
+000000c0: 0000 0000 0000 5a08 7901 7901 2300 6503  ......Z.y.y.#.e.
+000000d0: 2400 7205 0100 6401 5a02 5900 8c4c 7700  $.r...d.Z.Y..Lw.
+000000e0: 7803 5900 7701 2903 e900 0000 004e 6302  x.Y.w.)......Nc.
+000000f0: 0000 0000 0000 0000 0000 0005 0000 0003  ................
+00000100: 0000 00f3 2801 0000 9700 7c00 6a01 0000  ....(.....|.j...
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 6401 ab01 0000 0000 0000 7280 7403 0000  d.........r.t...
+00000130: 0000 0000 0000 6a04 0000 0000 0000 0000  ......j.........
+00000140: 0000 0000 0000 0000 0000 6402 7c00 7402  ..........d.|.t.
+00000150: 0000 0000 0000 0000 6a06 0000 0000 0000  ........j.......
+00000160: 0000 0000 0000 0000 0000 0000 ab03 0000  ................
+00000170: 0000 0000 7801 7d02 7259 7c00 7c02 6a09  ....x.}.rY|.|.j.
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 6403 ab01 0000 0000 0000 6400 1a00  ..d.........d...
+000001a0: 7d00 740b 0000 0000 0000 0000 6a0c 0000  }.t.........j...
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 7c02 6a0f 0000 0000 0000 0000 0000 0000  |.j.............
+000001d0: 0000 0000 0000 6404 ab01 0000 0000 0000  ......d.........
+000001e0: ab01 0000 0000 0000 7d03 7411 0000 0000  ........}.t.....
+000001f0: 0000 0000 7c03 7412 0000 0000 0000 0000  ....|.t.........
+00000200: ab02 0000 0000 0000 7211 7c01 6a15 0000  ........r.|.j...
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 7c03 ab01 0000 0000 0000 0100 7c00 5300  |...........|.S.
+00000230: 2905 4e7a 042d 2d2d 0a7a 125e 2d2d 2d5c  ).Nz.---.z.^---\
+00000240: 6e28 2e2a 3f5c 6e29 2d2d 2d5c 6e72 0200  n(.*?\n)---\nr..
+00000250: 0000 e901 0000 0029 0bda 0a73 7461 7274  .......)...start
+00000260: 7377 6974 68da 0272 65da 056d 6174 6368  swith..re..match
+00000270: da06 444f 5441 4c4c da03 656e 64da 0479  ..DOTALL..end..y
+00000280: 616d 6cda 0973 6166 655f 6c6f 6164 da05  aml..safe_load..
+00000290: 6772 6f75 70da 0a69 7369 6e73 7461 6e63  group..isinstanc
+000002a0: 65da 0464 6963 74da 0675 7064 6174 6529  e..dict..update)
+000002b0: 04da 0474 6578 74da 096d 6574 615f 6469  ...text..meta_di
+000002c0: 6374 7207 0000 00da 0464 6174 6173 0400  ctr......datas..
+000002d0: 0000 2020 2020 fa36 2f55 7365 7273 2f64  ..    .6/Users/d
+000002e0: 6d75 6c68 6f6c 6c2f 6465 762f 7372 632f  mulholl/dev/src/
+000002f0: 6172 6b2f 6172 6b2f 6578 7465 6e73 696f  ark/ark/extensio
+00000300: 6e73 2f61 726b 5f79 616d 6c2e 7079 da11  ns/ark_yaml.py..
+00000310: 7061 7273 655f 7961 6d6c 5f68 6561 6465  parse_yaml_heade
+00000320: 7272 1400 0000 0c00 0000 7372 0000 0080  rr........sr....
+00000330: 00e0 0b0f 8f3f 893f 9837 d40b 23dc 181a  .....?.?.7..#...
+00000340: 9f08 9908 d021 36b8 04bc 62bf 69b9 69d3  .....!6...b.i.i.
+00000350: 1848 d00f 4888 75d0 0f48 d817 1b98 459f  .H..H.u..H....E.
+00000360: 4999 49a0 619b 4c98 4dd0 172a 9004 dc17  I.I.a.L.M..*....
+00000370: 1b97 7e91 7ea0 65a7 6ba1 6bb0 21a3 6ed3  ..~.~.e.k.k.!.n.
+00000380: 1735 9004 dc13 1d98 64a4 44d4 1329 d814  .5......d.D..)..
+00000390: 1dd7 1424 d114 24a0 54d4 142a d80f 1388  ...$..$.T..*....
+000003a0: 0bf3 0000 0000 2909 da03 6172 6b72 0600  ......)...arkr..
+000003b0: 0000 720a 0000 00da 0b49 6d70 6f72 7445  ..r......ImportE
+000003c0: 7272 6f72 da07 6669 6c74 6572 73da 0872  rror..filters..r
+000003d0: 6567 6973 7465 72da 0646 696c 7465 72da  egister..Filter.
+000003e0: 0946 494c 455f 5445 5854 7214 0000 00a9  .FILE_TEXTr.....
+000003f0: 0072 1500 0000 7213 0000 00fa 083c 6d6f  .r....r......<mo
+00000400: 6475 6c65 3e72 1d00 0000 0100 0000 7366  dule>r........sf
+00000410: 0000 00f0 0301 0101 f306 0001 0bdb 0009  ................
+00000420: f004 0301 10db 040f f108 0004 08d8 0508  ................
+00000430: 875b 815b d705 19d1 0519 9823 9f2b 992b  .[.[.......#.+.+
+00000440: d71a 2cd1 1a2c d71a 36d1 1a36 d305 37f1  ..,..,..6..6..7.
+00000450: 0207 0514 f303 0006 38f1 0207 0514 f005  ........8.......
+00000460: 0004 08f8 f007 0008 13f2 0001 0110 d80b  ................
+00000470: 0f82 44f0 0301 0110 fa73 1100 0000 8a04  ..D......s......
+00000480: 4111 00c1 1107 411b 03c1 1a01 411b 03    A.....A.....A..
```

### Comparing `ark-7.1.0/ark/extensions/ark_automenu.py` & `ark-7.2.0/ark/extensions/ark_automenu.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/extensions/ark_jinja.py` & `ark-7.2.0/ark/extensions/ark_jinja.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/extensions/ark_shortcodes.py` & `ark-7.2.0/ark/extensions/ark_shortcodes.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/extensions/ark_yaml.py` & `ark-7.2.0/ark/extensions/ark_yaml.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/extensions.py` & `ark-7.2.0/ark/extensions.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/filters.py` & `ark-7.2.0/ark/filters.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/hashes.py` & `ark-7.2.0/ark/hashes.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/nodes.py` & `ark-7.2.0/ark/nodes.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/renderers.py` & `ark-7.2.0/ark/renderers.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/site.py` & `ark-7.2.0/ark/site.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/templates.py` & `ark-7.2.0/ark/templates.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark/utils.py` & `ark-7.2.0/ark/utils.py`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/ark.egg-info/PKG-INFO` & `ark-7.2.0/ark.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: ark
-Version: 7.1.0
+Version: 7.2.0
 Summary: A static website generator for people who enjoy the simpler things in life.
 Home-page: https://github.com/dmulholl/ark
 Author: Darren Mulholland
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Public Domain
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.8
+Requires-Dist: markdown~=3.0
+Requires-Dist: pygments~=2.0
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: jinja2~=3.0
+Requires-Dist: syntext~=3.0
+Requires-Dist: ibis~=3.0
+Requires-Dist: shortcodes~=5.1
+Requires-Dist: argslib~=2.0
+Requires-Dist: colorama~=0.4
 
 
 A static website generator for people who enjoy the simpler things in life.
 
 * `Github <https://github.com/dmulholl/ark>`_
 * `Documentation <http://www.dmulholl.com/docs/ark/main/>`_
 * `Demo <http://www.dmulholl.com/demos/ark/>`_
```

### Comparing `ark-7.1.0/ark.egg-info/SOURCES.txt` & `ark-7.2.0/ark.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,23 +15,26 @@
 ark/utils.py
 ark.egg-info/PKG-INFO
 ark.egg-info/SOURCES.txt
 ark.egg-info/dependency_links.txt
 ark.egg-info/entry_points.txt
 ark.egg-info/requires.txt
 ark.egg-info/top_level.txt
+ark/bundle/.DS_Store
 ark/bundle/site.py
 ark/bundle/inc/menu.md
+ark/bundle/lib/.DS_Store
 ark/bundle/lib/debug/license.txt
 ark/bundle/lib/debug/readme.md
 ark/bundle/lib/debug/resources/debug.css
 ark/bundle/lib/debug/resources/pygments.css
 ark/bundle/lib/debug/templates/node.ibis
 ark/bundle/lib/graphite/license.txt
 ark/bundle/lib/graphite/readme.md
+ark/bundle/lib/graphite/resources/assets/code.js
 ark/bundle/lib/graphite/resources/assets/fonts.css
 ark/bundle/lib/graphite/resources/assets/graphite.css
 ark/bundle/lib/graphite/resources/assets/pygments.css
 ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
 ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
 ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
 ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
@@ -63,14 +66,14 @@
 ark/extensions/ark_automenu.py
 ark/extensions/ark_ibis.py
 ark/extensions/ark_jinja.py
 ark/extensions/ark_markdown.py
 ark/extensions/ark_shortcodes.py
 ark/extensions/ark_syntext.py
 ark/extensions/ark_yaml.py
-ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
-ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
-ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
-ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
-ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
-ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
-ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
+ark/extensions/__pycache__/ark_automenu.cpython-312.pyc
+ark/extensions/__pycache__/ark_ibis.cpython-312.pyc
+ark/extensions/__pycache__/ark_jinja.cpython-312.pyc
+ark/extensions/__pycache__/ark_markdown.cpython-312.pyc
+ark/extensions/__pycache__/ark_shortcodes.cpython-312.pyc
+ark/extensions/__pycache__/ark_syntext.cpython-312.pyc
+ark/extensions/__pycache__/ark_yaml.cpython-312.pyc
```

### Comparing `ark-7.1.0/license.txt` & `ark-7.2.0/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.1.0/setup.py` & `ark-7.2.0/setup.py`

 * *Files identical despite different names*

