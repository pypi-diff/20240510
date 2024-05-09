# Comparing `tmp/simpleworkspace-1.2.197.tar.gz` & `tmp/simpleworkspace-1.2.198.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.197.tar", last modified: Thu May  9 14:39:16 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.198.tar", last modified: Thu May  9 23:17:22 2024, max compression
```

## Comparing `simpleworkspace-1.2.197.tar` & `simpleworkspace-1.2.198.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.492360 simpleworkspace-1.2.197/
--rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-05-09 14:39:16.487835 simpleworkspace-1.2.197/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-09 14:38:05.000000 simpleworkspace-1.2.197/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 14:39:16.494358 simpleworkspace-1.2.197/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.319019 simpleworkspace-1.2.197/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.351174 simpleworkspace-1.2.197/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:28:40.000000 simpleworkspace-1.2.197/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.363195 simpleworkspace-1.2.197/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.365199 simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.323635 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.367193 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.370186 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.377680 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.381671 simpleworkspace-1.2.197/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.387170 simpleworkspace-1.2.197/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.391160 simpleworkspace-1.2.197/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.397656 simpleworkspace-1.2.197/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.401646 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2966 2024-05-09 13:43:33.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6179 2024-05-09 14:36:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.408143 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0     9009 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.197/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.337695 simpleworkspace-1.2.197/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.409140 simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.332707 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.333706 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.412133 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.414127 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.415630 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.416636 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.423618 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.427154 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5067 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.436634 simpleworkspace-1.2.197/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.477296 simpleworkspace-1.2.197/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-24 12:00:58.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-03-10 14:41:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.483845 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3408 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.443439 simpleworkspace-1.2.198/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.198/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-05-09 23:17:22.441964 simpleworkspace-1.2.198/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-09 23:15:46.000000 simpleworkspace-1.2.198/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 23:17:22.443439 simpleworkspace-1.2.198/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.074854 simpleworkspace-1.2.198/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.157881 simpleworkspace-1.2.198/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.198/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.186539 simpleworkspace-1.2.198/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.195289 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.085959 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.201769 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.230926 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.256875 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.264079 simpleworkspace-1.2.198/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.198/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.279014 simpleworkspace-1.2.198/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.288382 simpleworkspace-1.2.198/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.198/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.301633 simpleworkspace-1.2.198/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.311085 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2999 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6179 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.327911 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0    13593 2024-05-09 23:11:21.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.198/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.198/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.198/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.125816 simpleworkspace-1.2.198/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.329977 simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.115582 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.117421 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.339451 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.342553 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.344814 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.350645 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.364693 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.376973 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.198/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.397696 simpleworkspace-1.2.198/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.198/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.433968 simpleworkspace-1.2.198/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.198/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:17:22.438787 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-05-09 23:17:22.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 23:17:21.000000 simpleworkspace-1.2.198/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/app.py` & `simpleworkspace-1.2.198/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0x2c98dc65 (Mon Feb 26 13:54:52 2024 UTC)
+moddate:  0xe803da65 (Sat Feb 24 14:57:44 2024 UTC)
 files sz: 561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -91,11 +91,11 @@
       '/audio/notifications/Completed.wav'
       '/audio/notifications/Error.wav'
       None
    names      ('os', 'path', '_path', 'dirname', 'abspath', '__file__', 'PATH_ASSETS', 'Icons_ErrorCircle_PNG', 'Icons_QuestionCircle_PNG', 'Icons_WarningCircle_PNG', 'Icons_InfoCircle_PNG', 'Audio_Alarms_Siren', 'Audio_Notification_Completed', 'Audio_Notification_Error')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Documents\\Development\\PythonProjects\\Py_SimpleWorkspace\\src\\simpleworkspace\\assets\\__init__.py'
+   filename   'C:\\dev\\pythonProjects\\Python_SimpleWorkspace\\src\\simpleworkspace\\assets\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0244020a010a010a010a020a010a01
```

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.198/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.198/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.198/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.198/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.198/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,19 +53,20 @@
             
             if not data:
                 break
 
             yield data
     return
 
-def Hash(filePath: str, hashFunc=_hashlib.md5()) -> str:
+def Hash(filePath: str, hashFn=_hashlib.sha1) -> str:
     from simpleworkspace.types.byte import ByteEnum
+    hashObj:_hashlib._Hash = hashFn()
     for data in ReadIterator(filePath, readSize=ByteEnum.KiloByte.value * 500, type=bytes):
-        hashFunc.update(data)
-    return hashFunc.hexdigest()
+        hashObj.update(data)
+    return hashObj.hexdigest()
     
 def Create(filepath: str, data: bytes | str = None):
     '''Creates or overwrites file if exists'''
 
     if type(data) is str:
         data = data.encode()
     with open(filepath, "wb") as file:
```

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.198/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.198/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.198/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.198/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.198/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.198/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.198/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.198/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.198/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.198/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.198/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.197/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.198/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/simpleworkspace/settingsproviders.py
 src/simpleworkspace.egg-info/PKG-INFO
 src/simpleworkspace.egg-info/SOURCES.txt
 src/simpleworkspace.egg-info/dependency_links.txt
 src/simpleworkspace.egg-info/requires.txt
 src/simpleworkspace.egg-info/top_level.txt
 src/simpleworkspace/assets/__init__.py
+src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
 src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
 src/simpleworkspace/assets/audio/alarms/Siren.wav
 src/simpleworkspace/assets/audio/notifications/Completed.wav
 src/simpleworkspace/assets/audio/notifications/Error.wav
 src/simpleworkspace/assets/icons/ErrorCircle.png
 src/simpleworkspace/assets/icons/InfoCircle.png
 src/simpleworkspace/assets/icons/QuestionCircle.png
```

