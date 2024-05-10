# Comparing `tmp/simpleworkspace-1.2.198.tar.gz` & `tmp/simpleworkspace-1.2.199.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.198.tar", last modified: Thu May  9 23:17:22 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.199.tar", last modified: Thu May  9 23:42:47 2024, max compression
```

## Comparing `simpleworkspace-1.2.198.tar` & `simpleworkspace-1.2.199.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.443439 simpleworkspace-1.2.198/
--rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.198/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-05-09 23:17:22.441964 simpleworkspace-1.2.198/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-09 23:15:46.000000 simpleworkspace-1.2.198/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 23:17:22.443439 simpleworkspace-1.2.198/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.074854 simpleworkspace-1.2.198/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.157881 simpleworkspace-1.2.198/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.198/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.186539 simpleworkspace-1.2.198/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.195289 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.085959 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.201769 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.230926 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.256875 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.264079 simpleworkspace-1.2.198/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.279014 simpleworkspace-1.2.198/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.288382 simpleworkspace-1.2.198/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.301633 simpleworkspace-1.2.198/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.311085 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2999 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6179 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.327911 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0    13593 2024-05-09 23:11:21.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.198/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.198/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.125816 simpleworkspace-1.2.198/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.329977 simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.115582 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.117421 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.339451 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.342553 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.344814 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.350645 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.364693 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.376973 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.198/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.397696 simpleworkspace-1.2.198/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.433968 simpleworkspace-1.2.198/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.438787 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-05-09 23:17:22.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:47.273507 simpleworkspace-1.2.199/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.199/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-05-09 23:42:47.266388 simpleworkspace-1.2.199/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-09 23:39:53.000000 simpleworkspace-1.2.199/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 23:42:47.276288 simpleworkspace-1.2.199/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:45.905259 simpleworkspace-1.2.199/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.017898 simpleworkspace-1.2.199/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.199/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.199/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.199/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.061326 simpleworkspace-1.2.199/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.068079 simpleworkspace-1.2.199/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:45.913726 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.076046 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.098992 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.127366 simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.154596 simpleworkspace-1.2.199/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.199/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.202382 simpleworkspace-1.2.199/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.199/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.199/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.199/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.228030 simpleworkspace-1.2.199/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.199/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.199/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.266080 simpleworkspace-1.2.199/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.296932 simpleworkspace-1.2.199/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2999 2024-05-09 18:37:59.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6179 2024-05-09 18:37:59.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.338942 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0    13603 2024-05-09 23:36:38.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.199/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.199/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.199/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:45.941441 simpleworkspace-1.2.199/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.353561 simpleworkspace-1.2.199/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:45.933028 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:45.934441 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.384079 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.401539 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.422091 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.426386 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.507691 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.554805 simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.199/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:46.885621 simpleworkspace-1.2.199/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.199/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:47.253910 simpleworkspace-1.2.199/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.199/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:42:47.260117 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-05-09 23:42:45.000000 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-05-09 23:42:45.000000 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 23:42:45.000000 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 23:42:45.000000 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 23:42:45.000000 simpleworkspace-1.2.199/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/app.py` & `simpleworkspace-1.2.199/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.199/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.199/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.199/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.199/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.199/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/readers/archive.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/readers/archive.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,21 +39,23 @@
         return outputPath
 
     @classmethod
     def Scan(cls, inputPath:str):
         import gzip, io
         
         with gzip.open(inputPath, mode='rb') as archive:
-            entry = _ArchiveEntry()
-            entry.IsDirectory = False
-            entry.Path = _os.path.basename(inputPath)
-            entry.Id = entry.Path
             archive.seek(0, io.SEEK_END)
-            entry.Size = archive.tell()
-            entry._dataContext = _ArchiveEntry._LazyIO(lambda: gzip.open(inputPath, mode='rb'))
+            entry = _ArchiveEntry(
+                path = _os.path.basename(inputPath),
+                size=archive.tell(),
+                isDirectory = False
+            )
+            entry._dataLoader = _ArchiveEntry._LazyIO(
+                FileHandleFactory=lambda: gzip.open(inputPath, mode='rb')
+            )
         return entry
 
 
 class TAR:
     @staticmethod
     def Create(inputPath: str, outputPath: str = None, pipe_gz=True, ignoreErrors=False):
         """Compresses file or folder to TAR or Tar+GZIP archive
@@ -117,21 +119,21 @@
     @classmethod
     def Scan(cls, inputPath:str):
         import tarfile
 
         extension, mode = cls._GetArchiveType(inputPath)
         with tarfile.open(inputPath, mode=mode) as archive:
             for entry in archive:
-                abstractEntry = _ArchiveEntry()
-                abstractEntry.IsDirectory = entry.isdir()
-                abstractEntry.Path = entry.name
-                abstractEntry.Id = abstractEntry.Path
-                abstractEntry.Size = entry.size
+                abstractEntry = _ArchiveEntry(
+                    path = entry.name,
+                    size = entry.size,
+                    isDirectory = entry.isdir()
+                )
                 if(abstractEntry.IsFile):
-                    abstractEntry._dataContext = _ArchiveEntry._LazyIO(
+                    abstractEntry._dataLoader = _ArchiveEntry._LazyIO(
                         FileHandleFactory=lambda: archive.extractfile(entry),
                     )
                 yield abstractEntry
 
 
     @classmethod
     def _GetArchiveType(cls, archivePath: str):
@@ -201,21 +203,21 @@
     
     @classmethod
     def Scan(cls, inputPath:str):
         import zipfile
 
         with zipfile.ZipFile(inputPath, mode="r") as archive:
             for entry in archive.filelist:
-                abstractEntry = _ArchiveEntry()
-                abstractEntry.IsDirectory = entry.is_dir()
-                abstractEntry.Path = entry.filename
-                abstractEntry.Id = abstractEntry.Path
-                abstractEntry.Size = entry.file_size
+                abstractEntry = _ArchiveEntry(
+                    path = entry.filename,
+                    size = entry.file_size,
+                    isDirectory = entry.is_dir(),
+                )
                 if(abstractEntry.IsFile):
-                    abstractEntry._dataContext = _ArchiveEntry._LazyIO(
+                    abstractEntry._dataLoader = _ArchiveEntry._LazyIO(
                         FileHandleFactory=lambda: archive.open(entry),
                     )
                 yield abstractEntry
 
 
 class SevenZip:
     @staticmethod
@@ -278,51 +280,51 @@
 
     @classmethod
     def Scan(cls, inputPath:str, password:str=None):
         import py7zr  # pip install py7zr
 
         with py7zr.SevenZipFile(inputPath, mode="r", password=password) as archive:
             for entry in archive.files:
-                abstractEntry = _ArchiveEntry()
-                abstractEntry.IsDirectory = entry.is_directory
-                abstractEntry.Path = entry.filename
-                abstractEntry.Id = str(entry.id)
-                abstractEntry.Size = entry.uncompressed
+                abstractEntry = _ArchiveEntry(
+                    path=entry.filename,
+                    id = str(entry.id),
+                    size = entry.uncompressed,
+                    isDirectory=entry.is_directory,
+                )
                 if(abstractEntry.IsFile):
-                    abstractEntry._dataContext = _ArchiveEntry._LazyIO(
+                    abstractEntry._dataLoader = _ArchiveEntry._LazyIO(
                         FileHandleFactory=lambda: archive.read(entry.filename)[entry.filename],
                         onClosedEvent=lambda: archive.reset()
                     )
                 yield abstractEntry
 
 
 class _ArchiveEntry:
-    Path:str
-    Id:str
-    Size:int
-
-    IsDirectory = False
-    @property 
-    def IsFile(self):
-        return self.IsDirectory == False
+    def __init__(self, path: str, id:str=None, size:int=None, isDirectory=False) -> None:
+        self.Path = path.rstrip('/\\')
+        self.Id = self.Path if id is None else id
+        self.Size = size
+        self.IsDirectory = isDirectory
+        self.IsFile = isDirectory == False
+
 
-    _dataContext:'_LazyIO'
     def DataReader(self):
         '''
         Gets an io stream of archive data, is used with context manager
         >>> with entry.ReadData() as stream:...
         '''
-        return self._dataContext
+        return self._dataLoader
     
     @property
     def Data(self):
         '''Loads the complete file data into memory'''
         with self.DataReader() as stream:
             return stream.read()
     
+    _dataLoader:'_LazyIO'
     class _LazyIO:
         def __init__(self, FileHandleFactory:_Callable[[], _BinaryIO], onClosedEvent:_Callable = None):
             self._openFn = FileHandleFactory
             self._io:_BinaryIO
             self._onClosedEvent = onClosedEvent
 
         def __enter__(self):
```

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.199/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.199/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.199/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.199/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.199/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.199/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.199/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.199/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.199/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.199/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.199/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.198/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.199/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

