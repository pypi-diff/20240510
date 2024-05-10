# Comparing `tmp/autoboot-0.6.0.tar.gz` & `tmp/autoboot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot-0.6.0.tar", last modified: Thu Nov 30 02:17:46 2023, max compression
+gzip compressed data, was "autoboot-0.7.0.tar", last modified: Thu Nov 30 10:21:14 2023, max compression
```

## Comparing `autoboot-0.6.0.tar` & `autoboot-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.460194 autoboot-0.6.0/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-0.6.0/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:56:55.000000 autoboot-0.6.0/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)      678 2023-11-30 02:17:46.460300 autoboot-0.6.0/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)      116 2023-11-15 09:22:25.000000 autoboot-0.6.0/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.445161 autoboot-0.6.0/autoboot/
--rw-r--r--   0 yizzuide   (501) staff       (20)      243 2023-11-25 09:26:51.000000 autoboot-0.6.0/autoboot/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.450963 autoboot-0.6.0/autoboot/annotation/
--rw-r--r--   0 yizzuide   (501) staff       (20)      200 2023-11-21 10:08:01.000000 autoboot-0.6.0/autoboot/annotation/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1578 2023-11-25 10:01:04.000000 autoboot-0.6.0/autoboot/annotation/component.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      804 2023-11-23 09:22:19.000000 autoboot-0.6.0/autoboot/annotation/effect.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1189 2023-11-24 07:19:38.000000 autoboot-0.6.0/autoboot/annotation/env.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1149 2023-11-22 02:16:54.000000 autoboot-0.6.0/autoboot/annotation/log.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      660 2023-11-25 09:09:07.000000 autoboot-0.6.0/autoboot/application_properties.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     3216 2023-11-29 02:28:21.000000 autoboot-0.6.0/autoboot/applications.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      735 2023-11-18 02:00:00.000000 autoboot-0.6.0/autoboot/args.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.451511 autoboot-0.6.0/autoboot/event/
--rw-r--r--   0 yizzuide   (501) staff       (20)      177 2023-11-22 02:16:54.000000 autoboot-0.6.0/autoboot/event/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1289 2023-11-24 06:17:20.000000 autoboot-0.6.0/autoboot/event/event_emitter.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2497 2023-11-22 02:16:54.000000 autoboot-0.6.0/autoboot/logging.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.452589 autoboot-0.6.0/autoboot/meta/
--rw-r--r--   0 yizzuide   (501) staff       (20)      100 2023-09-23 12:35:52.000000 autoboot-0.6.0/autoboot/meta/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      416 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/meta/component.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      526 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/meta/component_metaclass.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      169 2023-09-23 12:42:36.000000 autoboot-0.6.0/autoboot/meta/property.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.453500 autoboot-0.6.0/autoboot/plugin/
--rw-r--r--   0 yizzuide   (501) staff       (20)       77 2023-11-29 02:28:21.000000 autoboot-0.6.0/autoboot/plugin/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      362 2023-11-29 02:28:21.000000 autoboot-0.6.0/autoboot/plugin/app_plugin.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.454629 autoboot-0.6.0/autoboot/process/
--rw-r--r--   0 yizzuide   (501) staff       (20)      840 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/process/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      370 2023-11-29 02:28:21.000000 autoboot-0.6.0/autoboot/process/env_process.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1445 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/process/yaml_constructors.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      728 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/process/yaml_parser.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      537 2023-11-27 02:09:47.000000 autoboot-0.6.0/autoboot/server_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.455228 autoboot-0.6.0/autoboot/thread/
--rw-r--r--   0 yizzuide   (501) staff       (20)       70 2023-11-25 09:39:12.000000 autoboot-0.6.0/autoboot/thread/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1514 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/thread/thread_pool.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.456975 autoboot-0.6.0/autoboot/util/
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-16 02:54:04.000000 autoboot-0.6.0/autoboot/util/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2712 2023-11-30 02:17:32.000000 autoboot-0.6.0/autoboot/util/capacity.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      302 2023-11-17 07:31:30.000000 autoboot-0.6.0/autoboot/util/json_model.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      560 2023-11-17 06:29:28.000000 autoboot-0.6.0/autoboot/util/local_cache.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      504 2023-11-14 09:04:15.000000 autoboot-0.6.0/autoboot/util/object_navigator.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1092 2023-11-22 07:00:40.000000 autoboot-0.6.0/autoboot/util/type_reflect.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.447522 autoboot-0.6.0/autoboot.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)      678 2023-11-30 02:17:46.000000 autoboot-0.6.0/autoboot.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)     1321 2023-11-30 02:17:46.000000 autoboot-0.6.0/autoboot.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 02:17:46.000000 autoboot-0.6.0/autoboot.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)      129 2023-11-30 02:17:46.000000 autoboot-0.6.0/autoboot.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        9 2023-11-30 02:17:46.000000 autoboot-0.6.0/autoboot.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-15 07:41:11.000000 autoboot-0.6.0/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 02:17:46.460699 autoboot-0.6.0/setup.cfg
--rw-r--r--   0 yizzuide   (501) staff       (20)     1201 2023-11-30 02:17:32.000000 autoboot-0.6.0/setup.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.459343 autoboot-0.6.0/tests/
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:05:15.000000 autoboot-0.6.0/tests/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      810 2023-11-24 06:13:20.000000 autoboot-0.6.0/tests/test_event_emitter.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:17:46.459971 autoboot-0.6.0/tests/test_ioc_properties/
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:05:15.000000 autoboot-0.6.0/tests/test_ioc_properties/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      256 2023-11-30 02:17:32.000000 autoboot-0.6.0/tests/test_ioc_properties/test_ioc_properties.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      523 2023-11-20 06:17:50.000000 autoboot-0.6.0/tests/test_json_model.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      137 2023-11-17 06:18:39.000000 autoboot-0.6.0/tests/test_pipy_repo.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      350 2023-11-24 06:20:43.000000 autoboot-0.6.0/tests/test_retry.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.707649 autoboot-0.7.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-0.7.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:56:55.000000 autoboot-0.7.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)      678 2023-11-30 10:21:14.707773 autoboot-0.7.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)      116 2023-11-15 09:22:25.000000 autoboot-0.7.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.689041 autoboot-0.7.0/autoboot/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      243 2023-11-25 09:26:51.000000 autoboot-0.7.0/autoboot/__init__.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.693854 autoboot-0.7.0/autoboot/annotation/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      200 2023-11-21 10:08:01.000000 autoboot-0.7.0/autoboot/annotation/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1665 2023-11-30 09:28:44.000000 autoboot-0.7.0/autoboot/annotation/component.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      804 2023-11-23 09:22:19.000000 autoboot-0.7.0/autoboot/annotation/effect.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1189 2023-11-30 07:20:26.000000 autoboot-0.7.0/autoboot/annotation/env.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1149 2023-11-22 02:16:54.000000 autoboot-0.7.0/autoboot/annotation/log.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      799 2023-11-30 09:38:07.000000 autoboot-0.7.0/autoboot/application_properties.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     4339 2023-11-30 09:42:18.000000 autoboot-0.7.0/autoboot/applications.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      735 2023-11-18 02:00:00.000000 autoboot-0.7.0/autoboot/args.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.696047 autoboot-0.7.0/autoboot/event/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      325 2023-11-30 08:56:48.000000 autoboot-0.7.0/autoboot/event/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      245 2023-11-30 09:27:02.000000 autoboot-0.7.0/autoboot/event/application_listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      173 2023-11-30 09:17:22.000000 autoboot-0.7.0/autoboot/event/component_listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1289 2023-11-24 06:17:20.000000 autoboot-0.7.0/autoboot/event/event_emitter.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2497 2023-11-22 02:16:54.000000 autoboot-0.7.0/autoboot/logging.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.699037 autoboot-0.7.0/autoboot/meta/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      143 2023-11-30 09:44:03.000000 autoboot-0.7.0/autoboot/meta/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      416 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/meta/component.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      526 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/meta/component_metaclass.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      353 2023-11-30 09:46:42.000000 autoboot-0.7.0/autoboot/meta/listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      169 2023-09-23 12:42:36.000000 autoboot-0.7.0/autoboot/meta/property.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.700153 autoboot-0.7.0/autoboot/plugin/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       60 2023-11-30 03:14:32.000000 autoboot-0.7.0/autoboot/plugin/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1059 2023-11-30 08:26:53.000000 autoboot-0.7.0/autoboot/plugin/app_plugin.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      285 2023-11-30 02:52:47.000000 autoboot-0.7.0/autoboot/plugin/app_plugin_metaclass.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.701693 autoboot-0.7.0/autoboot/process/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      840 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/process/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      370 2023-11-29 02:28:21.000000 autoboot-0.7.0/autoboot/process/env_process.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1445 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/process/yaml_constructors.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      728 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/process/yaml_parser.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      537 2023-11-27 02:09:47.000000 autoboot-0.7.0/autoboot/server_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.702742 autoboot-0.7.0/autoboot/thread/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       70 2023-11-25 09:39:12.000000 autoboot-0.7.0/autoboot/thread/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1514 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/thread/thread_pool.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.705007 autoboot-0.7.0/autoboot/util/
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-16 02:54:04.000000 autoboot-0.7.0/autoboot/util/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2712 2023-11-30 02:17:32.000000 autoboot-0.7.0/autoboot/util/capacity.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      302 2023-11-17 07:31:30.000000 autoboot-0.7.0/autoboot/util/json_model.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      560 2023-11-17 06:29:28.000000 autoboot-0.7.0/autoboot/util/local_cache.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      504 2023-11-14 09:04:15.000000 autoboot-0.7.0/autoboot/util/object_navigator.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1092 2023-11-22 07:00:40.000000 autoboot-0.7.0/autoboot/util/type_reflect.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.690557 autoboot-0.7.0/autoboot.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      678 2023-11-30 10:21:14.000000 autoboot-0.7.0/autoboot.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1463 2023-11-30 10:21:14.000000 autoboot-0.7.0/autoboot.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 10:21:14.000000 autoboot-0.7.0/autoboot.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)      129 2023-11-30 10:21:14.000000 autoboot-0.7.0/autoboot.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        9 2023-11-30 10:21:14.000000 autoboot-0.7.0/autoboot.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-15 07:41:11.000000 autoboot-0.7.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 10:21:14.708203 autoboot-0.7.0/setup.cfg
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1201 2023-11-30 10:03:15.000000 autoboot-0.7.0/setup.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.706723 autoboot-0.7.0/tests/
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:05:15.000000 autoboot-0.7.0/tests/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      810 2023-11-24 06:13:20.000000 autoboot-0.7.0/tests/test_event_emitter.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:21:14.707333 autoboot-0.7.0/tests/test_ioc_properties/
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-30 09:40:23.000000 autoboot-0.7.0/tests/test_ioc_properties/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      258 2023-11-30 09:52:12.000000 autoboot-0.7.0/tests/test_ioc_properties/test_ioc_properties.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      523 2023-11-20 06:17:50.000000 autoboot-0.7.0/tests/test_json_model.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      137 2023-11-17 06:18:39.000000 autoboot-0.7.0/tests/test_pipy_repo.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      350 2023-11-24 06:20:43.000000 autoboot-0.7.0/tests/test_retry.py
```

### Comparing `autoboot-0.6.0/LICENSE.txt` & `autoboot-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/PKG-INFO` & `autoboot-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot
-Version: 0.6.0
+Version: 0.7.0
 Summary: IoC with auto config framework
 Home-page: https://github.com/yizzuide/autoboot
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: IoC,event,auto config
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-0.6.0/autoboot/annotation/component.py` & `autoboot-0.7.0/autoboot/annotation/component.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 R = TypeVar("R")
 
 def comp_from_cache(name: str, comp_factory: Callable[..., R]):
   """
   Get component from cache
   """
  
-  app: AutoBoot = AutoBoot.instance()
+  app = AutoBoot.instance()
   # return cached component if match
   for key, comp in app.components:
     if key == name:
       return comp
   comp = comp_factory()
+  
+  for listener in app._component_listeners:
+    listener.after_instantiation(name, comp)
+    
   # caching component with name
   if comp:
     app.components.append((name, comp))
     (AutoBoot.logger or logger).info(f"component cached: {name}")
   return comp
 
 def component(name: str):
```

### Comparing `autoboot-0.6.0/autoboot/annotation/effect.py` & `autoboot-0.7.0/autoboot/annotation/effect.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/annotation/env.py` & `autoboot-0.7.0/autoboot/annotation/env.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/annotation/log.py` & `autoboot-0.7.0/autoboot/annotation/log.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/application_properties.py` & `autoboot-0.7.0/autoboot/application_properties.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     return "app"
 
   @value_component("autoboot.application.module")
   @staticmethod
   def module() -> str:
     return "api"
   
+  @value_component("autoboot.application.scan_listener_packages")
+  @staticmethod
+  def scan_listener_packages() -> list[str]:
+    pass
+  
   @value_component("autoboot.application.log.dir")
   @staticmethod
   def log_dir() -> str:
     return "logs"
   
   @value_component("autoboot.application.log.max_size")
   @staticmethod
```

### Comparing `autoboot-0.6.0/autoboot/args.py` & `autoboot-0.7.0/autoboot/args.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/event/event_emitter.py` & `autoboot-0.7.0/autoboot/event/event_emitter.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/logging.py` & `autoboot-0.7.0/autoboot/logging.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/meta/component_metaclass.py` & `autoboot-0.7.0/autoboot/meta/component_metaclass.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/process/__init__.py` & `autoboot-0.7.0/autoboot/process/__init__.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/process/yaml_constructors.py` & `autoboot-0.7.0/autoboot/process/yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/process/yaml_parser.py` & `autoboot-0.7.0/autoboot/process/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/server_properties.py` & `autoboot-0.7.0/autoboot/server_properties.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/thread/thread_pool.py` & `autoboot-0.7.0/autoboot/thread/thread_pool.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/util/capacity.py` & `autoboot-0.7.0/autoboot/util/capacity.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/util/local_cache.py` & `autoboot-0.7.0/autoboot/util/local_cache.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot/util/type_reflect.py` & `autoboot-0.7.0/autoboot/util/type_reflect.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/autoboot.egg-info/PKG-INFO` & `autoboot-0.7.0/autoboot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot
-Version: 0.6.0
+Version: 0.7.0
 Summary: IoC with auto config framework
 Home-page: https://github.com/yizzuide/autoboot
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: IoC,event,auto config
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-0.6.0/autoboot.egg-info/SOURCES.txt` & `autoboot-0.7.0/autoboot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,25 @@
 autoboot.egg-info/top_level.txt
 autoboot/annotation/__init__.py
 autoboot/annotation/component.py
 autoboot/annotation/effect.py
 autoboot/annotation/env.py
 autoboot/annotation/log.py
 autoboot/event/__init__.py
+autoboot/event/application_listener.py
+autoboot/event/component_listener.py
 autoboot/event/event_emitter.py
 autoboot/meta/__init__.py
 autoboot/meta/component.py
 autoboot/meta/component_metaclass.py
+autoboot/meta/listener.py
 autoboot/meta/property.py
 autoboot/plugin/__init__.py
 autoboot/plugin/app_plugin.py
+autoboot/plugin/app_plugin_metaclass.py
 autoboot/process/__init__.py
 autoboot/process/env_process.py
 autoboot/process/yaml_constructors.py
 autoboot/process/yaml_parser.py
 autoboot/thread/__init__.py
 autoboot/thread/thread_pool.py
 autoboot/util/__init__.py
```

### Comparing `autoboot-0.6.0/pyproject.toml` & `autoboot-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/setup.py` & `autoboot-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.6.0'
+VERSION = '0.7.0'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='autoboot',
     version=VERSION,
```

### Comparing `autoboot-0.6.0/tests/test_event_emitter.py` & `autoboot-0.7.0/tests/test_event_emitter.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.6.0/tests/test_json_model.py` & `autoboot-0.7.0/tests/test_json_model.py`

 * *Files identical despite different names*

