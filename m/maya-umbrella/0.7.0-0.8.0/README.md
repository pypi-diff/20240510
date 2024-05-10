# Comparing `tmp/maya_umbrella-0.7.0.tar.gz` & `tmp/maya_umbrella-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.7.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.8.0.tar", max compression
```

## Comparing `maya_umbrella-0.7.0.tar` & `maya_umbrella-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-05-09 06:15:50.725921 maya_umbrella-0.7.0/LICENSE
--rw-r--r--   0        0        0     9796 2024-05-09 06:15:50.725921 maya_umbrella-0.7.0/README.md
--rw-r--r--   0        0        0      401 2024-05-09 06:15:50.749920 maya_umbrella-0.7.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-09 06:15:50.749920 maya_umbrella-0.7.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0     5044 2024-05-09 06:15:50.749920 maya_umbrella-0.7.0/maya_umbrella/cleaner.py
--rw-r--r--   0        0        0    13111 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/collector.py
--rw-r--r--   0        0        0      539 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/constants.py
--rw-r--r--   0        0        0     5601 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/defender.py
--rw-r--r--   0        0        0     8333 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      761 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1281 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      556 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      484 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     2683 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/i18n.py
--rw-r--r--   0        0        0      962 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/locales/en_US.json
--rw-r--r--   0        0        0     1006 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/locales/zh_CN.json
--rw-r--r--   0        0        0     1338 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/log.py
--rw-r--r--   0        0        0     3645 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/maya_funs.py
--rw-r--r--   0        0        0     3921 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/scanner.py
--rw-r--r--   0        0        0      354 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/signatures.py
--rw-r--r--   0        0        0     1022 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      489 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2123 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3493 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     5285 2024-05-09 06:15:50.753920 maya_umbrella-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10847 1970-01-01 00:00:00.000000 maya_umbrella-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 12:32:55.351753 maya_umbrella-0.8.0/LICENSE
+-rw-r--r--   0        0        0     9945 2024-05-10 12:32:55.351753 maya_umbrella-0.8.0/README.md
+-rw-r--r--   0        0        0      401 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0     5044 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/cleaner.py
+-rw-r--r--   0        0        0    13111 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/collector.py
+-rw-r--r--   0        0        0      539 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     5601 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/defender.py
+-rw-r--r--   0        0        0     8333 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1281 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      556 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      484 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     2683 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/i18n.py
+-rw-r--r--   0        0        0      962 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/locales/en_US.json
+-rw-r--r--   0        0        0     1006 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/locales/zh_CN.json
+-rw-r--r--   0        0        0     1338 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/log.py
+-rw-r--r--   0        0        0     3645 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/maya_funs.py
+-rw-r--r--   0        0        0     3921 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/scanner.py
+-rw-r--r--   0        0        0      354 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/signatures.py
+-rw-r--r--   0        0        0     1022 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2123 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3493 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     5285 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10996 1970-01-01 00:00:00.000000 maya_umbrella-0.8.0/PKG-INFO
```

### Comparing `maya_umbrella-0.7.0/LICENSE` & `maya_umbrella-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/README.md` & `maya_umbrella-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,20 @@
 MAYA_UMBRELLA_LANG
 ```
 
 忽略保存到备份文件夹，*请注意，如果你不清楚这个会导致的后果请不要轻易修改*，默认批量杀毒后会把源文件自动备份到当前文件的备份文件夹.
 ```shell
 MAYA_UMBRELLA_IGNORE_BACKUP
 ```
+
+如果是便携版Maya，可以通过添加 `MAYA_LOCATION` 环境变量指定Maya路径
+```shell
+SET MAYA_LOCATION=d:/your/path/maya_version/
+```
+
 如果忽略请设置为
 ```shell
 SET MAYA_UMBRELLA_IGNORE_BACKUP=true
 ```
 
 # API
 获取当前场景没有被修复的病毒文件
```

### Comparing `maya_umbrella-0.7.0/maya_umbrella/cleaner.py` & `maya_umbrella-0.8.0/maya_umbrella/cleaner.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/collector.py` & `maya_umbrella-0.8.0/maya_umbrella/collector.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/constants.py` & `maya_umbrella-0.8.0/maya_umbrella/constants.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/defender.py` & `maya_umbrella-0.8.0/maya_umbrella/defender.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/filesystem.py` & `maya_umbrella-0.8.0/maya_umbrella/filesystem.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.8.0/maya_umbrella/hooks/delete_turtle.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.8.0/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.8.0/maya_umbrella/hooks/fix_model_panel.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/i18n.py` & `maya_umbrella-0.8.0/maya_umbrella/i18n.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/locales/en_US.json` & `maya_umbrella-0.8.0/maya_umbrella/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/locales/zh_CN.json` & `maya_umbrella-0.8.0/maya_umbrella/locales/zh_CN.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/log.py` & `maya_umbrella-0.8.0/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/maya_funs.py` & `maya_umbrella-0.8.0/maya_umbrella/maya_funs.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/scanner.py` & `maya_umbrella-0.8.0/maya_umbrella/scanner.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/vaccine.py` & `maya_umbrella-0.8.0/maya_umbrella/vaccine.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine2.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine3.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.7.0/pyproject.toml` & `maya_umbrella-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.7.0"
+version = "0.8.0"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -32,15 +32,15 @@
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = { version = "^2024.3.2", python = ">=3.8.1,<3.11" }
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.8.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
```

### Comparing `maya_umbrella-0.7.0/PKG-INFO` & `maya_umbrella-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_umbrella
-Version: 0.7.0
+Version: 0.8.0
 Summary: Check and fix maya virus.
 Home-page: https://github.com/loonghao/maya_umbrella
 License: MIT
 Keywords: notifiers,python,Maya,dcc
 Author: longhao
 Author-email: hal.long@outlook.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
@@ -150,14 +150,20 @@
 MAYA_UMBRELLA_LANG
 ```
 
 忽略保存到备份文件夹，*请注意，如果你不清楚这个会导致的后果请不要轻易修改*，默认批量杀毒后会把源文件自动备份到当前文件的备份文件夹.
 ```shell
 MAYA_UMBRELLA_IGNORE_BACKUP
 ```
+
+如果是便携版Maya，可以通过添加 `MAYA_LOCATION` 环境变量指定Maya路径
+```shell
+SET MAYA_LOCATION=d:/your/path/maya_version/
+```
+
 如果忽略请设置为
 ```shell
 SET MAYA_UMBRELLA_IGNORE_BACKUP=true
 ```
 
 # API
 获取当前场景没有被修复的病毒文件
```

