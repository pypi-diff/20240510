# Comparing `tmp/bhbot-2.2.tar.gz` & `tmp/bhbot-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhbot-2.2.tar", last modified: Fri Apr 26 19:39:00 2024, max compression
+gzip compressed data, was "bhbot-2.3.tar", last modified: Fri May 10 19:56:21 2024, max compression
```

## Comparing `bhbot-2.2.tar` & `bhbot-2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:39:00.511493 bhbot-2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:39:00.511493 bhbot-2.2/BHBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:39:00.000000 bhbot-2.2/BHBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-26 19:38:56.000000 bhbot-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 19:39:00.511493 bhbot-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-26 19:38:56.000000 bhbot-2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-26 19:38:56.000000 bhbot-2.2/abstract_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-26 19:38:56.000000 bhbot-2.2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-26 19:38:56.000000 bhbot-2.2/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 19:38:56.000000 bhbot-2.2/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-26 19:38:56.000000 bhbot-2.2/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-26 19:38:56.000000 bhbot-2.2/direct_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 19:38:56.000000 bhbot-2.2/font_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-26 19:38:56.000000 bhbot-2.2/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-26 19:38:56.000000 bhbot-2.2/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-26 19:38:56.000000 bhbot-2.2/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 19:38:56.000000 bhbot-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:39:00.511493 bhbot-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-26 19:38:56.000000 bhbot-2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 19:38:56.000000 bhbot-2.2/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-26 19:38:56.000000 bhbot-2.2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-26 19:38:56.000000 bhbot-2.2/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:56:21.304597 bhbot-2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:56:21.304597 bhbot-2.3/BHBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-10 19:56:21.000000 bhbot-2.3/BHBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 19:56:21.000000 bhbot-2.3/BHBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:56:21.000000 bhbot-2.3/BHBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:56:21.000000 bhbot-2.3/BHBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-10 19:56:17.000000 bhbot-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-10 19:56:21.304597 bhbot-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-10 19:56:17.000000 bhbot-2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-10 19:56:17.000000 bhbot-2.3/abstract_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-05-10 19:56:17.000000 bhbot-2.3/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-10 19:56:17.000000 bhbot-2.3/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:56:17.000000 bhbot-2.3/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-05-10 19:56:17.000000 bhbot-2.3/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-10 19:56:17.000000 bhbot-2.3/direct_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 19:56:17.000000 bhbot-2.3/font_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-05-10 19:56:17.000000 bhbot-2.3/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-10 19:56:17.000000 bhbot-2.3/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-10 19:56:17.000000 bhbot-2.3/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 19:56:17.000000 bhbot-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:56:21.304597 bhbot-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 19:56:17.000000 bhbot-2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 19:56:17.000000 bhbot-2.3/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-10 19:56:17.000000 bhbot-2.3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-10 19:56:17.000000 bhbot-2.3/windows.py
```

### Comparing `bhbot-2.2/LICENSE` & `bhbot-2.3/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-Unlicense
 This is free and unencumbered software released into the public domain.
 
 Anyone is free to copy, modify, publish, use, compile, sell, or
 distribute this software, either in source code form or as a compiled
 binary, for any purpose, commercial or non-commercial, and by any
 means.
```

### Comparing `bhbot-2.2/abstract_mode.py` & `bhbot-2.3/abstract_mode.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/bot.py` & `bhbot-2.3/bot.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/characters.py` & `bhbot-2.3/characters.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/config.py` & `bhbot-2.3/config.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/direct_input.py` & `bhbot-2.3/direct_input.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/font_loader.py` & `bhbot-2.3/font_loader.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/gui.py` & `bhbot-2.3/gui.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/levels.py` & `bhbot-2.3/levels.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/menu.py` & `bhbot-2.3/menu.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/utils.py` & `bhbot-2.3/utils.py`

 * *Files identical despite different names*

### Comparing `bhbot-2.2/windows.py` & `bhbot-2.3/windows.py`

 * *Files identical despite different names*

