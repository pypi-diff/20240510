# Comparing `tmp/poke_donpollo-2.0.1.tar.gz` & `tmp/poke_donpollo-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poke_donpollo-2.0.1.tar", last modified: Fri Apr 26 03:41:48 2024, max compression
+gzip compressed data, was "poke_donpollo-2.0.5.tar", last modified: Fri May 10 00:38:51 2024, max compression
```

## Comparing `poke_donpollo-2.0.1.tar` & `poke_donpollo-2.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:41:48.737726 poke_donpollo-2.0.1/
--rw-rw-rw-   0        0        0      228 2024-04-26 03:41:48.735637 poke_donpollo-2.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 03:41:48.720984 poke_donpollo-2.0.1/POKE_DONPOLLO/
--rw-rw-rw-   0        0        0       43 2024-04-19 15:35:51.000000 poke_donpollo-2.0.1/POKE_DONPOLLO/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:19:52.000000 poke_donpollo-2.0.1/POKE_DONPOLLO/pokemon.csv
--rw-rw-rw-   0        0        0     2408 2024-04-24 03:46:11.000000 poke_donpollo-2.0.1/POKE_DONPOLLO/ramdom_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:41:48.733568 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/
--rw-rw-rw-   0        0        0      228 2024-04-26 03:41:48.000000 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-26 03:41:48.000000 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:41:48.000000 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 03:41:48.000000 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-26 03:41:48.000000 poke_donpollo-2.0.1/POKE_DONPOLLO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2024-04-26 02:49:54.000000 poke_donpollo-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 03:41:48.737726 poke_donpollo-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-26 03:41:31.000000 poke_donpollo-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:38:51.876309 poke_donpollo-2.0.5/
+-rw-rw-rw-   0        0        0      228 2024-05-10 00:38:51.874209 poke_donpollo-2.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 00:38:51.858505 poke_donpollo-2.0.5/POKE_DONPOLLO/
+-rw-rw-rw-   0        0        0       43 2024-04-19 15:35:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:19:52.000000 poke_donpollo-2.0.5/POKE_DONPOLLO/pokemon.csv
+-rw-rw-rw-   0        0        0     2408 2024-04-24 03:46:11.000000 poke_donpollo-2.0.5/POKE_DONPOLLO/ramdom_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:38:51.872110 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-10 00:38:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-10 00:38:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:38:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 00:38:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 00:38:51.000000 poke_donpollo-2.0.5/POKE_DONPOLLO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2024-04-26 02:49:54.000000 poke_donpollo-2.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:38:51.876309 poke_donpollo-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-10 00:38:42.000000 poke_donpollo-2.0.5/setup.py
```

### Comparing `poke_donpollo-2.0.1/POKE_DONPOLLO/pokemon.csv` & `poke_donpollo-2.0.5/POKE_DONPOLLO/pokemon.csv`

 * *Files identical despite different names*

### Comparing `poke_donpollo-2.0.1/POKE_DONPOLLO/ramdom_pokemon.py` & `poke_donpollo-2.0.5/POKE_DONPOLLO/ramdom_pokemon.py`

 * *Files identical despite different names*

