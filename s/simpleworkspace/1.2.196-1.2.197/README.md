# Comparing `tmp/simpleworkspace-1.2.196.tar.gz` & `tmp/simpleworkspace-1.2.197.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.196.tar", last modified: Thu May  9 14:07:11 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.197.tar", last modified: Thu May  9 14:39:16 2024, max compression
```

## Comparing `simpleworkspace-1.2.196.tar` & `simpleworkspace-1.2.197.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.406985 simpleworkspace-1.2.196/
--rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-05-09 14:07:11.404991 simpleworkspace-1.2.196/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-09 14:06:00.000000 simpleworkspace-1.2.196/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 14:07:11.406985 simpleworkspace-1.2.196/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.241214 simpleworkspace-1.2.196/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.271258 simpleworkspace-1.2.196/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.196/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:28:40.000000 simpleworkspace-1.2.196/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.284300 simpleworkspace-1.2.196/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.286294 simpleworkspace-1.2.196/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.245211 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.287291 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.302415 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.308919 simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.313433 simpleworkspace-1.2.196/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.196/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.196/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.196/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.319925 simpleworkspace-1.2.196/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.196/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.196/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.196/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.323426 simpleworkspace-1.2.196/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.196/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.196/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.331441 simpleworkspace-1.2.196/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.335946 simpleworkspace-1.2.196/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2966 2024-05-09 13:43:33.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6037 2024-05-09 14:04:17.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.343441 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0     9009 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.196/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.196/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.196/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.259273 simpleworkspace-1.2.196/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.344439 simpleworkspace-1.2.196/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.254765 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.254765 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.347956 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.349950 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.350948 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.352455 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.360957 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-17 14:57:41.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.364457 simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5067 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.196/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.375470 simpleworkspace-1.2.196/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.401990 simpleworkspace-1.2.196/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-12 17:24:38.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-24 12:00:58.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-03-10 14:41:22.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.196/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:07:11.403994 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-09 14:07:11.000000 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3408 2024-05-09 14:07:11.000000 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:07:11.000000 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 14:07:11.000000 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 14:07:11.000000 simpleworkspace-1.2.196/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.492360 simpleworkspace-1.2.197/
+-rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-05-09 14:39:16.487835 simpleworkspace-1.2.197/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-09 14:38:05.000000 simpleworkspace-1.2.197/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:39:16.494358 simpleworkspace-1.2.197/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.319019 simpleworkspace-1.2.197/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.351174 simpleworkspace-1.2.197/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:28:40.000000 simpleworkspace-1.2.197/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.363195 simpleworkspace-1.2.197/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.365199 simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.323635 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.367193 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.370186 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.377680 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.381671 simpleworkspace-1.2.197/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.197/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.387170 simpleworkspace-1.2.197/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.391160 simpleworkspace-1.2.197/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.397656 simpleworkspace-1.2.197/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.401646 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2966 2024-05-09 13:43:33.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6179 2024-05-09 14:36:30.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.408143 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0     9009 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.197/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.197/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.337695 simpleworkspace-1.2.197/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.409140 simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.332707 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.333706 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.412133 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.414127 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.415630 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.416636 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.423618 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.427154 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5067 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.436634 simpleworkspace-1.2.197/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.477296 simpleworkspace-1.2.197/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-12 17:24:38.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-24 12:00:58.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-03-10 14:41:22.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.197/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:39:16.483845 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3408 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 14:39:16.000000 simpleworkspace-1.2.197/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/app.py` & `simpleworkspace-1.2.197/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.197/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.197/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.197/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.197/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.197/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     def IsSymlink(self) -> bool:
         return _os.path.islink(self.Path)
     
     @property
     def Exists(self) -> bool:
         return _os.path.exists(self.Path)
     
-    def Join(self, *otherPaths:str):
+    def Join(self, *otherPaths:'str|PathInfo'):
+        otherPaths = [str(x) if type(x) is PathInfo else x for x in otherPaths] #convert pathinfo objects to str aswell
         return self.__class__(_os.path.join(self.Path, *otherPaths), self._normalizePath)
 
     @property
     def Stats(self):
         return _os.stat(self.Path) #follows symlink by default
 
     @_cached_property
@@ -131,15 +132,15 @@
     
     def __str__(self):
         return self.Path
     
     def _NormalizePathIfNeeded(self, path:str):
         return path.replace("\\", "/") if self._normalizePath else path
     
-    def __truediv__(self, otherPath:str):
+    def __truediv__(self, otherPath:'str|PathInfo'):
         return self.Join(otherPath)
     
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             return NotImplemented
         #could also have been swapped for abspath to make different path syntax match aswell...
         return self.Path == other.Path
```

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/readers/archive.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/readers/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.197/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.197/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.197/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.197/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.197/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.197/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.197/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.197/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.197/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.197/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.197/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.196/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.197/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

