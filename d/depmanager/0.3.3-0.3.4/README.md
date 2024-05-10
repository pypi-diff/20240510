# Comparing `tmp/depmanager-0.3.3.tar.gz` & `tmp/depmanager-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depmanager-0.3.3.tar", last modified: Sat Jan 27 12:43:44 2024, max compression
+gzip compressed data, was "depmanager-0.3.4.tar", last modified: Fri May 10 07:56:54 2024, max compression
```

## Comparing `depmanager-0.3.3.tar` & `depmanager-0.3.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.392813 depmanager-0.3.3/
--rw-rw-rw-   0        0        0     1085 2024-01-15 23:11:23.000000 depmanager-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    20503 2024-01-27 12:43:44.390646 depmanager-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    18568 2024-01-27 12:43:01.000000 depmanager-0.3.3/README.md
--rw-rw-rw-   0        0        0     1072 2024-01-27 12:42:59.000000 depmanager-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-27 12:43:44.393912 depmanager-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.262277 depmanager-0.3.3/src/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.273219 depmanager-0.3.3/src/depmanager/
--rw-rw-rw-   0        0        0      150 2023-12-02 22:55:44.000000 depmanager-0.3.3/src/depmanager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.314119 depmanager-0.3.3/src/depmanager/api/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.3/src/depmanager/api/__init__.py
--rw-rw-rw-   0        0        0    11737 2024-01-19 08:42:23.000000 depmanager-0.3.3/src/depmanager/api/builder.py
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.362033 depmanager-0.3.3/src/depmanager/api/internal/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.3/src/depmanager/api/internal/__init__.py
--rw-rw-rw-   0        0        0     5413 2023-12-11 21:05:22.000000 depmanager-0.3.3/src/depmanager/api/internal/common.py
--rw-rw-rw-   0        0        0     3414 2024-01-10 20:29:11.000000 depmanager-0.3.3/src/depmanager/api/internal/config_file.py
--rw-rw-rw-   0        0        0     2982 2024-01-10 20:29:11.000000 depmanager-0.3.3/src/depmanager/api/internal/data_locking.py
--rw-rw-rw-   0        0        0     8435 2024-01-19 07:45:25.000000 depmanager-0.3.3/src/depmanager/api/internal/database_common.py
--rw-rw-rw-   0        0        0     2469 2023-12-02 22:55:44.000000 depmanager-0.3.3/src/depmanager/api/internal/database_local.py
--rw-rw-rw-   0        0        0     2527 2023-12-04 08:40:35.000000 depmanager-0.3.3/src/depmanager/api/internal/database_remote_folder.py
--rw-rw-rw-   0        0        0     3696 2023-12-04 08:41:02.000000 depmanager-0.3.3/src/depmanager/api/internal/database_remote_ftp.py
--rw-rw-rw-   0        0        0    14090 2023-12-11 21:05:22.000000 depmanager-0.3.3/src/depmanager/api/internal/database_remote_server.py
--rw-rw-rw-   0        0        0    20029 2024-01-27 00:53:14.000000 depmanager-0.3.3/src/depmanager/api/internal/dependency.py
--rw-rw-rw-   0        0        0     2624 2023-12-04 08:38:33.000000 depmanager-0.3.3/src/depmanager/api/internal/machine.py
--rw-rw-rw-   0        0        0    11053 2024-01-25 22:51:55.000000 depmanager-0.3.3/src/depmanager/api/internal/recipe_builder.py
--rw-rw-rw-   0        0        0    12137 2024-01-10 20:29:11.000000 depmanager-0.3.3/src/depmanager/api/internal/system.py
--rw-rw-rw-   0        0        0     5981 2024-01-10 20:29:11.000000 depmanager-0.3.3/src/depmanager/api/load.py
--rw-rw-rw-   0        0        0     1288 2024-01-27 12:42:59.000000 depmanager-0.3.3/src/depmanager/api/local.py
--rw-rw-rw-   0        0        0     8202 2024-01-10 20:29:11.000000 depmanager-0.3.3/src/depmanager/api/package.py
--rw-rw-rw-   0        0        0     2354 2024-01-15 22:55:26.000000 depmanager-0.3.3/src/depmanager/api/recipe.py
--rw-rw-rw-   0        0        0    15372 2023-12-12 16:36:14.000000 depmanager-0.3.3/src/depmanager/api/remotes.py
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.365500 depmanager-0.3.3/src/depmanager/cmake/
--rw-rw-rw-   0        0        0     6841 2024-01-19 07:45:25.000000 depmanager-0.3.3/src/depmanager/cmake/DepManager.cmake
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.386201 depmanager-0.3.3/src/depmanager/command/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.3/src/depmanager/command/__init__.py
--rw-rw-rw-   0        0        0     4496 2024-01-15 22:55:26.000000 depmanager-0.3.3/src/depmanager/command/build.py
--rw-rw-rw-   0        0        0     1623 2023-12-12 16:36:14.000000 depmanager-0.3.3/src/depmanager/command/get.py
--rw-rw-rw-   0        0        0     1876 2024-01-10 20:29:12.000000 depmanager-0.3.3/src/depmanager/command/info.py
--rw-rw-rw-   0        0        0     4121 2024-01-10 20:29:12.000000 depmanager-0.3.3/src/depmanager/command/load.py
--rw-rw-rw-   0        0        0     6315 2024-01-27 12:42:59.000000 depmanager-0.3.3/src/depmanager/command/pack.py
--rw-rw-rw-   0        0        0     6807 2023-12-12 16:36:14.000000 depmanager-0.3.3/src/depmanager/command/remote.py
--rw-rw-rw-   0        0        0     1926 2024-01-10 20:29:12.000000 depmanager-0.3.3/src/depmanager/manager.py
-drwxrwxrwx   0        0        0        0 2024-01-27 12:43:44.388376 depmanager-0.3.3/src/depmanager.egg-info/
--rw-rw-rw-   0        0        0    20503 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-01-27 12:43:44.000000 depmanager-0.3.3/src/depmanager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.592521 depmanager-0.3.4/
+-rw-rw-rw-   0        0        0     1085 2024-01-15 23:11:23.000000 depmanager-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    20669 2024-05-10 07:56:54.590519 depmanager-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    18734 2024-05-10 07:55:41.000000 depmanager-0.3.4/README.md
+-rw-rw-rw-   0        0        0     1072 2024-05-10 07:55:41.000000 depmanager-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 07:56:54.592521 depmanager-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.448523 depmanager-0.3.4/src/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.455522 depmanager-0.3.4/src/depmanager/
+-rw-rw-rw-   0        0        0      150 2023-12-02 22:55:44.000000 depmanager-0.3.4/src/depmanager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.498523 depmanager-0.3.4/src/depmanager/api/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.4/src/depmanager/api/__init__.py
+-rw-rw-rw-   0        0        0    11737 2024-01-19 08:42:23.000000 depmanager-0.3.4/src/depmanager/api/builder.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.554519 depmanager-0.3.4/src/depmanager/api/internal/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.4/src/depmanager/api/internal/__init__.py
+-rw-rw-rw-   0        0        0     5413 2023-12-11 21:05:22.000000 depmanager-0.3.4/src/depmanager/api/internal/common.py
+-rw-rw-rw-   0        0        0     3414 2024-01-10 20:29:11.000000 depmanager-0.3.4/src/depmanager/api/internal/config_file.py
+-rw-rw-rw-   0        0        0     2982 2024-01-10 20:29:11.000000 depmanager-0.3.4/src/depmanager/api/internal/data_locking.py
+-rw-rw-rw-   0        0        0     8435 2024-01-19 07:45:25.000000 depmanager-0.3.4/src/depmanager/api/internal/database_common.py
+-rw-rw-rw-   0        0        0     2469 2023-12-02 22:55:44.000000 depmanager-0.3.4/src/depmanager/api/internal/database_local.py
+-rw-rw-rw-   0        0        0     2527 2023-12-04 08:40:35.000000 depmanager-0.3.4/src/depmanager/api/internal/database_remote_folder.py
+-rw-rw-rw-   0        0        0     3696 2023-12-04 08:41:02.000000 depmanager-0.3.4/src/depmanager/api/internal/database_remote_ftp.py
+-rw-rw-rw-   0        0        0    14090 2023-12-11 21:05:22.000000 depmanager-0.3.4/src/depmanager/api/internal/database_remote_server.py
+-rw-rw-rw-   0        0        0    20029 2024-01-27 00:53:14.000000 depmanager-0.3.4/src/depmanager/api/internal/dependency.py
+-rw-rw-rw-   0        0        0     2624 2023-12-04 08:38:33.000000 depmanager-0.3.4/src/depmanager/api/internal/machine.py
+-rw-rw-rw-   0        0        0    11071 2024-04-01 18:31:25.000000 depmanager-0.3.4/src/depmanager/api/internal/recipe_builder.py
+-rw-rw-rw-   0        0        0    12137 2024-01-10 20:29:11.000000 depmanager-0.3.4/src/depmanager/api/internal/system.py
+-rw-rw-rw-   0        0        0     5981 2024-01-10 20:29:11.000000 depmanager-0.3.4/src/depmanager/api/load.py
+-rw-rw-rw-   0        0        0     1288 2024-05-10 07:55:41.000000 depmanager-0.3.4/src/depmanager/api/local.py
+-rw-rw-rw-   0        0        0     8202 2024-01-10 20:29:11.000000 depmanager-0.3.4/src/depmanager/api/package.py
+-rw-rw-rw-   0        0        0     2354 2024-01-15 22:55:26.000000 depmanager-0.3.4/src/depmanager/api/recipe.py
+-rw-rw-rw-   0        0        0    15372 2023-12-12 16:36:14.000000 depmanager-0.3.4/src/depmanager/api/remotes.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.559520 depmanager-0.3.4/src/depmanager/cmake/
+-rw-rw-rw-   0        0        0     6841 2024-01-19 07:45:25.000000 depmanager-0.3.4/src/depmanager/cmake/DepManager.cmake
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.585516 depmanager-0.3.4/src/depmanager/command/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.3.4/src/depmanager/command/__init__.py
+-rw-rw-rw-   0        0        0     4496 2024-01-15 22:55:26.000000 depmanager-0.3.4/src/depmanager/command/build.py
+-rw-rw-rw-   0        0        0     1623 2023-12-12 16:36:14.000000 depmanager-0.3.4/src/depmanager/command/get.py
+-rw-rw-rw-   0        0        0     1876 2024-01-10 20:29:12.000000 depmanager-0.3.4/src/depmanager/command/info.py
+-rw-rw-rw-   0        0        0     4121 2024-01-10 20:29:12.000000 depmanager-0.3.4/src/depmanager/command/load.py
+-rw-rw-rw-   0        0        0     7001 2024-05-10 07:55:41.000000 depmanager-0.3.4/src/depmanager/command/pack.py
+-rw-rw-rw-   0        0        0     6807 2023-12-12 16:36:14.000000 depmanager-0.3.4/src/depmanager/command/remote.py
+-rw-rw-rw-   0        0        0     1926 2024-01-10 20:29:12.000000 depmanager-0.3.4/src/depmanager/manager.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:56:54.588519 depmanager-0.3.4/src/depmanager.egg-info/
+-rw-rw-rw-   0        0        0    20669 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-10 07:56:54.000000 depmanager-0.3.4/src/depmanager.egg-info/top_level.txt
```

### Comparing `depmanager-0.3.3/LICENSE` & `depmanager-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/PKG-INFO` & `depmanager-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depmanager
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple Dependency manager
 Author-email: Silmaen <genteur.slayer@laposte.net>
 License: MIT License
         
         Copyright (c) 2024 Silmaen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -220,42 +220,42 @@
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
 
 Here is a small cmake code snippet to initialize depmanager in cmake.
 
 ```cmake
 # add HINTS or PATH to find the executable if not in the PATH
-find_program(EDEPMANAGER depmanager) 
+find_program(EDEPMANAGER depmanager)
 if (${EDEPMANAGER} STREQUAL EDEPMANAGER-NOTFOUND)
     message(FATAL_ERROR "Dependency manager not found.")
-else()
+else ()
     execute_process(COMMAND ${EDEPMANAGER} info cmakedir
             OUTPUT_VARIABLE depmanager_path)
     string(STRIP ${depmanager_path} depmanager_path)
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
-endif()
+endif ()
 ```
 
 ### Automated mode
 
 In automated mode, depmanager can automatically set a remote repository, retrieve packages from this repository
 and load then in one command.
 
 #### The command
 
 ```cmake
 dm_load_environment(
-   [QUIET]
-   [PATH path]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        [QUIET]
+        [PATH path]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 ) 
 ```
 
 If `QUIET` set, only errors are written.
 
 `path` is the path to the configuration file, either directly a configuration file name,
 or a directory containing a file named `depmanager.yml`. By default, it will look at the
@@ -318,22 +318,22 @@
 #### Find packages
 
 With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
-   package
-   [QUIET] [TRACE] [REQUIRED]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [QUIET] [TRACE] [REQUIRED]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
@@ -355,22 +355,22 @@
 #### Load package
 
 This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
-   package
-   [REQUIRED] [TRACE]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [REQUIRED] [TRACE]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
@@ -469,16 +469,18 @@
         * [ ] Searching across remotes with final package sorting.
         * [ ] Allow auto-pull best-fitting package
 * version 0.4.x
     * [ ] Add concept of toolset.
         * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
         * [ ] Use toolset in build.
         * [ ] Use toolset in queries.
-    * [ ] More detail documentation.
-        * [ ] Documentation hosted in instance of [Depmanager Server](https://github.com/Silmaen/DepManagerServer).
+* version 0.3.4 -- 2024-05-08
+    * [X] bugfix: deepcopy in push command (for multiple push)
+    * [X] bugfix: quotes in Cmake invocation command
+    * [X] Add more verbose output in cleaning command
 * version 0.3.3 -- 2024-01-27
     * [X] Improved Builder Configurations management
     * [X] Operation on multiple package
         * [X] add a 'clean' command
             * [X] basic mode: keep only the newest packages
             * [X] full mode: delete everything.
         * [X] allow local deletion of multiple packages
@@ -497,15 +499,15 @@
 * version 0.3.0 -- 2024-01-12
     * [X] CMake integration improvement
         * [X] Simplify integration with cmake
         * [X] Python auto generate the Module dir for cmake
         * [X] Allow to load package by batch
             * [X] use Yaml config file.
 * version 0.2.1 -- 2023-12-31
-    * [X] Bufix: allow more date format and don't break if bad format.
+    * [X] Bugfix: allow more date format and don't break if bad format.
 * version 0.2.0 -- 2023-12-12
     * WARNING: Some breaking change. Backward compatibility not fully tested.
     * [X] Faster commandline
         * [X] Use remote connexion only if needed
     * [X] Transitive search
         * [X] Query: search in local then remote.
         * [X] get: Auto-pull if not in local.
```

### Comparing `depmanager-0.3.3/README.md` & `depmanager-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -179,42 +179,42 @@
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
 
 Here is a small cmake code snippet to initialize depmanager in cmake.
 
 ```cmake
 # add HINTS or PATH to find the executable if not in the PATH
-find_program(EDEPMANAGER depmanager) 
+find_program(EDEPMANAGER depmanager)
 if (${EDEPMANAGER} STREQUAL EDEPMANAGER-NOTFOUND)
     message(FATAL_ERROR "Dependency manager not found.")
-else()
+else ()
     execute_process(COMMAND ${EDEPMANAGER} info cmakedir
             OUTPUT_VARIABLE depmanager_path)
     string(STRIP ${depmanager_path} depmanager_path)
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
-endif()
+endif ()
 ```
 
 ### Automated mode
 
 In automated mode, depmanager can automatically set a remote repository, retrieve packages from this repository
 and load then in one command.
 
 #### The command
 
 ```cmake
 dm_load_environment(
-   [QUIET]
-   [PATH path]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        [QUIET]
+        [PATH path]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 ) 
 ```
 
 If `QUIET` set, only errors are written.
 
 `path` is the path to the configuration file, either directly a configuration file name,
 or a directory containing a file named `depmanager.yml`. By default, it will look at the
@@ -277,22 +277,22 @@
 #### Find packages
 
 With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
-   package
-   [QUIET] [TRACE] [REQUIRED]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [QUIET] [TRACE] [REQUIRED]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
@@ -314,22 +314,22 @@
 #### Load package
 
 This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
-   package
-   [REQUIRED] [TRACE]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [REQUIRED] [TRACE]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
@@ -428,16 +428,18 @@
         * [ ] Searching across remotes with final package sorting.
         * [ ] Allow auto-pull best-fitting package
 * version 0.4.x
     * [ ] Add concept of toolset.
         * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
         * [ ] Use toolset in build.
         * [ ] Use toolset in queries.
-    * [ ] More detail documentation.
-        * [ ] Documentation hosted in instance of [Depmanager Server](https://github.com/Silmaen/DepManagerServer).
+* version 0.3.4 -- 2024-05-08
+    * [X] bugfix: deepcopy in push command (for multiple push)
+    * [X] bugfix: quotes in Cmake invocation command
+    * [X] Add more verbose output in cleaning command
 * version 0.3.3 -- 2024-01-27
     * [X] Improved Builder Configurations management
     * [X] Operation on multiple package
         * [X] add a 'clean' command
             * [X] basic mode: keep only the newest packages
             * [X] full mode: delete everything.
         * [X] allow local deletion of multiple packages
@@ -456,15 +458,15 @@
 * version 0.3.0 -- 2024-01-12
     * [X] CMake integration improvement
         * [X] Simplify integration with cmake
         * [X] Python auto generate the Module dir for cmake
         * [X] Allow to load package by batch
             * [X] use Yaml config file.
 * version 0.2.1 -- 2023-12-31
-    * [X] Bufix: allow more date format and don't break if bad format.
+    * [X] Bugfix: allow more date format and don't break if bad format.
 * version 0.2.0 -- 2023-12-12
     * WARNING: Some breaking change. Backward compatibility not fully tested.
     * [X] Faster commandline
         * [X] Use remote connexion only if needed
     * [X] Transitive search
         * [X] Query: search in local then remote.
         * [X] get: Auto-pull if not in local.
```

### Comparing `depmanager-0.3.3/pyproject.toml` & `depmanager-0.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "depmanager"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     { name = "Silmaen", email = "genteur.slayer@laposte.net" }
 ]
 description = "Simple Dependency manager"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `depmanager-0.3.3/src/depmanager/api/builder.py` & `depmanager-0.3.4/src/depmanager/api/builder.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/common.py` & `depmanager-0.3.4/src/depmanager/api/internal/common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/config_file.py` & `depmanager-0.3.4/src/depmanager/api/internal/config_file.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/data_locking.py` & `depmanager-0.3.4/src/depmanager/api/internal/data_locking.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/database_common.py` & `depmanager-0.3.4/src/depmanager/api/internal/database_common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/database_local.py` & `depmanager-0.3.4/src/depmanager/api/internal/database_local.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/database_remote_folder.py` & `depmanager-0.3.4/src/depmanager/api/internal/database_remote_folder.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/database_remote_ftp.py` & `depmanager-0.3.4/src/depmanager/api/internal/database_remote_ftp.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/database_remote_server.py` & `depmanager-0.3.4/src/depmanager/api/internal/database_remote_server.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/dependency.py` & `depmanager-0.3.4/src/depmanager/api/internal/dependency.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/machine.py` & `depmanager-0.3.4/src/depmanager/api/internal/machine.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/recipe_builder.py` & `depmanager-0.3.4/src/depmanager/api/internal/recipe_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,39 +103,39 @@
                     file=stderr,
                 )
             return None
         return source_dir
 
     def _get_generator(self):
         if self.generator not in ["", None]:
-            return f" -G {self.generator}"
+            return f' -G "{self.generator}"'
         if len(self.recipe.config) > 1:
-            return " -G Ninja Multi-Config"
+            return ' -G "Ninja Multi-Config"'
         if len(self.recipe.config) == 1:
-            return " -G Ninja"
+            return ' -G "Ninja"'
         return ""
 
     def _get_configs(self):
         if len(self.recipe.config) > 1:
-            return f" -DCMAKE_CONFIGURATION_TYPES={';'.join(self.recipe.config)}"
+            return f' -DCMAKE_CONFIGURATION_TYPES="{";".join(self.recipe.config)}"'
         if len(self.recipe.config) == 1:
-            return f" -DCMAKE_BUILD_TYPE={self.recipe.config[0]}"
+            return f' -DCMAKE_BUILD_TYPE="{self.recipe.config[0]}"'
         return ""
 
     def _get_options_str(self):
-        out = f" -DCMAKE_INSTALL_PREFIX={self.temp / 'install'}"
+        out = f' -DCMAKE_INSTALL_PREFIX="{self.temp / "install"}"'
         out += f" -DBUILD_SHARED_LIBS={['OFF', 'ON'][self.recipe.kind.lower() == 'shared']}"
         if "C_COMPILER" in self.cross_info:
-            out += f" -DCMAKE_C_COMPILER={self.cross_info['C_COMPILER']}"
+            out += f' -DCMAKE_C_COMPILER="{self.cross_info["C_COMPILER"]}"'
         if "CXX_COMPILER" in self.cross_info:
-            out += f" -DCMAKE_CXX_COMPILER={self.cross_info['CXX_COMPILER']}"
+            out += f' -DCMAKE_CXX_COMPILER="{self.cross_info["CXX_COMPILER"]}"'
         if self.recipe.settings["os"].lower() in ["linux"]:
             out += " -DCMAKE_SKIP_INSTALL_RPATH=ON -DCMAKE_POSITION_INDEPENDENT_CODE=ON"
         for key, val in self.recipe.cache_variables.items():
-            out += f" -D{key}={val}"
+            out += f' -D{key}="{val}"'
         return out
 
     def _make_define(self):
         mac = Machine(True)
         self.creation_date = datetime.now(
             tz=datetime.now().astimezone().tzinfo
         ).replace(microsecond=0)
```

### Comparing `depmanager-0.3.3/src/depmanager/api/internal/system.py` & `depmanager-0.3.4/src/depmanager/api/internal/system.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/load.py` & `depmanager-0.3.4/src/depmanager/api/load.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/local.py` & `depmanager-0.3.4/src/depmanager/api/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class LocalManager:
     """
     Local manager.
     """
 
-    version = "0.3.3"
+    version = "0.3.4"
 
     def __init__(self, system=None, verbosity: int = 0):
         from depmanager.api.internal.system import LocalSystem
 
         self.verbosity = verbosity
         if type(system) is LocalSystem:
             self.__sys = system
```

### Comparing `depmanager-0.3.3/src/depmanager/api/package.py` & `depmanager-0.3.4/src/depmanager/api/package.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/recipe.py` & `depmanager-0.3.4/src/depmanager/api/recipe.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/api/remotes.py` & `depmanager-0.3.4/src/depmanager/api/remotes.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/cmake/DepManager.cmake` & `depmanager-0.3.4/src/depmanager/cmake/DepManager.cmake`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/command/build.py` & `depmanager-0.3.4/src/depmanager/command/build.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/command/get.py` & `depmanager-0.3.4/src/depmanager/command/get.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/command/info.py` & `depmanager-0.3.4/src/depmanager/command/info.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/command/load.py` & `depmanager-0.3.4/src/depmanager/command/load.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/command/pack.py` & `depmanager-0.3.4/src/depmanager/command/pack.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Pack command
 """
+from copy import deepcopy
 from pathlib import Path
 from sys import stderr
 
 possible_info = ["pull", "push", "add", "del", "query", "clean"]
 
 
 def pack(args, system=None):
@@ -83,26 +84,39 @@
     else:
         deps = pacman.query(query, remote_name, transitivity)
     if args.what == "query":
         for dep in deps:
             print(f"[{dep.get_source()}] {dep.properties.get_as_str()}")
         return
     if args.what == "clean":
+        if args.verbose > 0:
+            print(
+                f"Do a {['','full '][args.full]} Cleaning of the local package repository."
+            )
         if args.full:
             for dep in deps:
+                if args.verbose > 0:
+                    print(f"Remove package {dep.properties.get_as_str()}")
                 pacman.remove_package(dep, remote_name)
         else:
             for dep in deps:
                 props = dep.properties
                 props.version = "*"
                 result = pacman.query(props, remote_name)
                 if len(result) < 2:
+                    if args.verbose > 0:
+                        print(f"Keeping package {dep.properties.get_as_str()}")
                     continue
                 if result[0].version_greater(dep):
+                    if args.verbose > 0:
+                        print(f"Remove package {dep.properties.get_as_str()}")
                     pacman.remove_package(dep, remote_name)
+                else:
+                    if args.verbose > 0:
+                        print(f"Keeping package {dep.properties.get_as_str()}")
         return
     if args.what in ["del", "pull", "push"]:
         if len(deps) == 0:
             print("WARNING: No package matching the query.", file=stderr)
             return
         if len(deps) > 1 and not args.recurse:
             print(
@@ -112,15 +126,15 @@
             for dep in deps:
                 print(f"{dep.properties.get_as_str()}")
             return
         for dep in deps:
             if args.what == "del":
                 pacman.remove_package(dep, remote_name)
                 continue
-            props = dep.properties
+            props = deepcopy(dep.properties)
             props.version = "*"
             result = pacman.query(props, remote_name)
             if len(result) >= 2 and result[0].version_greater(dep):
                 continue
             if args.what == "pull":
                 pacman.add_from_remote(dep, remote_name)
             elif args.what == "push":
```

### Comparing `depmanager-0.3.3/src/depmanager/command/remote.py` & `depmanager-0.3.4/src/depmanager/command/remote.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager/manager.py` & `depmanager-0.3.4/src/depmanager/manager.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.3.3/src/depmanager.egg-info/PKG-INFO` & `depmanager-0.3.4/src/depmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depmanager
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple Dependency manager
 Author-email: Silmaen <genteur.slayer@laposte.net>
 License: MIT License
         
         Copyright (c) 2024 Silmaen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -220,42 +220,42 @@
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
 
 Here is a small cmake code snippet to initialize depmanager in cmake.
 
 ```cmake
 # add HINTS or PATH to find the executable if not in the PATH
-find_program(EDEPMANAGER depmanager) 
+find_program(EDEPMANAGER depmanager)
 if (${EDEPMANAGER} STREQUAL EDEPMANAGER-NOTFOUND)
     message(FATAL_ERROR "Dependency manager not found.")
-else()
+else ()
     execute_process(COMMAND ${EDEPMANAGER} info cmakedir
             OUTPUT_VARIABLE depmanager_path)
     string(STRIP ${depmanager_path} depmanager_path)
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
-endif()
+endif ()
 ```
 
 ### Automated mode
 
 In automated mode, depmanager can automatically set a remote repository, retrieve packages from this repository
 and load then in one command.
 
 #### The command
 
 ```cmake
 dm_load_environment(
-   [QUIET]
-   [PATH path]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        [QUIET]
+        [PATH path]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 ) 
 ```
 
 If `QUIET` set, only errors are written.
 
 `path` is the path to the configuration file, either directly a configuration file name,
 or a directory containing a file named `depmanager.yml`. By default, it will look at the
@@ -318,22 +318,22 @@
 #### Find packages
 
 With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
-   package
-   [QUIET] [TRACE] [REQUIRED]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [QUIET] [TRACE] [REQUIRED]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
@@ -355,22 +355,22 @@
 #### Load package
 
 This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
-   package
-   [REQUIRED] [TRACE]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-   [GLIBC target_glibc]
+        package
+        [REQUIRED] [TRACE]
+        [VERSION version]
+        [KIND kind]
+        [ARCH target_arch]
+        [OS target_os]
+        [COMPILER target_compiler]
+        [GLIBC target_glibc]
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
@@ -469,16 +469,18 @@
         * [ ] Searching across remotes with final package sorting.
         * [ ] Allow auto-pull best-fitting package
 * version 0.4.x
     * [ ] Add concept of toolset.
         * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
         * [ ] Use toolset in build.
         * [ ] Use toolset in queries.
-    * [ ] More detail documentation.
-        * [ ] Documentation hosted in instance of [Depmanager Server](https://github.com/Silmaen/DepManagerServer).
+* version 0.3.4 -- 2024-05-08
+    * [X] bugfix: deepcopy in push command (for multiple push)
+    * [X] bugfix: quotes in Cmake invocation command
+    * [X] Add more verbose output in cleaning command
 * version 0.3.3 -- 2024-01-27
     * [X] Improved Builder Configurations management
     * [X] Operation on multiple package
         * [X] add a 'clean' command
             * [X] basic mode: keep only the newest packages
             * [X] full mode: delete everything.
         * [X] allow local deletion of multiple packages
@@ -497,15 +499,15 @@
 * version 0.3.0 -- 2024-01-12
     * [X] CMake integration improvement
         * [X] Simplify integration with cmake
         * [X] Python auto generate the Module dir for cmake
         * [X] Allow to load package by batch
             * [X] use Yaml config file.
 * version 0.2.1 -- 2023-12-31
-    * [X] Bufix: allow more date format and don't break if bad format.
+    * [X] Bugfix: allow more date format and don't break if bad format.
 * version 0.2.0 -- 2023-12-12
     * WARNING: Some breaking change. Backward compatibility not fully tested.
     * [X] Faster commandline
         * [X] Use remote connexion only if needed
     * [X] Transitive search
         * [X] Query: search in local then remote.
         * [X] get: Auto-pull if not in local.
```

### Comparing `depmanager-0.3.3/src/depmanager.egg-info/SOURCES.txt` & `depmanager-0.3.4/src/depmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

