# Comparing `tmp/radical.utils-1.9.0.tar.gz` & `tmp/radical.utils-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.utils-1.9.0.tar", last modified: Tue Nov 23 17:35:07 2021, max compression
+gzip compressed data, was "dist/radical.utils-1.9.1.tar", last modified: Tue Dec 14 14:07:27 2021, max compression
```

## Comparing `radical.utils-1.9.0.tar` & `radical.utils-1.9.1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       72 2021-11-23 17:35:07.000000 radical.utils-1.9.0/setup.cfg
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/examples/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/examples/zmq/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/examples/zmq/queue/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      687 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/queue/get.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      662 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/queue/put.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1242 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/queue/queue.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3474 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/protocols.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2290 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/README.md
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/examples/zmq/pubsub/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      575 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/pubsub/pub.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      640 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/pubsub/pubsub.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      598 2021-09-24 08:23:31.000000 radical.utils-1.9.0/examples/zmq/pubsub/sub.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    24695 2021-11-23 17:34:45.000000 radical.utils-1.9.0/CHANGES.md
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9606 2021-11-23 17:33:31.000000 radical.utils-1.9.0/setup.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1210 2021-09-24 08:23:31.000000 radical.utils-1.9.0/README.md
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/bin/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5983 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-utils-mongodb.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      526 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-stack
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      168 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-utils-version
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5247 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-utils-fix-headers.pl
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     7354 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/ru.json.sh
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5581 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-utils-pwatch
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      328 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-utils-pylint.sh
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)    11855 2021-11-23 17:33:31.000000 radical.utils-1.9.0/bin/radical-utils-env.sh
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2695 2021-09-24 08:23:31.000000 radical.utils-1.9.0/bin/radical-bridge
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1285 2021-09-24 08:23:31.000000 radical.utils-1.9.0/LICENSE.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1014 2021-11-23 17:35:07.000000 radical.utils-1.9.0/PKG-INFO
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/test_cases/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4110 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/test_cases/host.00000.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2024 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/test_cases/ids.00000.json
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/bin/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      998 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/bin/ru-runcheck.sh
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/unittests/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4860 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_ids.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3293 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/unittests/test_zmq_client.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3227 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_object_cache.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5016 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/unittests/test_host.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1993 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_json.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2280 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_plugin_manager.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1370 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_regex.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4278 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_lockfile.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/__init__.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3060 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_zmq_pubsub.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4399 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_dict_mixin.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1358 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/unittests/test_zmq_registry.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1258 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_signatures.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1273 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_locks.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9022 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_zmq_queue.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4643 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_algorithms.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/unittests/data/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      469 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/data/import_file.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       99 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/data/resource_yale.json
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      923 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_singleton.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3806 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_lease_manager.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1447 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_poll.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4552 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_logger.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2959 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_read_json.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8610 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_misc.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2311 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_time.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1806 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_daemonize.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1579 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_config.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4573 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_profiler.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2962 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_description.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3571 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_heartbeat.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3354 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_lockable.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      781 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_which.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4006 2021-11-23 16:26:24.000000 radical.utils-1.9.0/tests/unittests/test_env.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2121 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/unittests/test_stack.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     7528 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_url.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3712 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_reporter.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)    10261 2021-11-23 17:33:31.000000 radical.utils-1.9.0/tests/unittests/test_munch.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/tests/integration_tests/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3114 2021-09-24 08:23:31.000000 radical.utils-1.9.0/tests/integration_tests/test_flux.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-11-23 17:34:51.000000 radical.utils-1.9.0/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      107 2021-09-24 08:23:31.000000 radical.utils-1.9.0/MANIFEST.in
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       80 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/top_level.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1014 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4600 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical.utils.egg-info/SOURCES.txt
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    27801 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/profile.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       41 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/SDIST
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3160 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/tracer.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/atfork/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3088 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/atfork/stdlib_fixer.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2022 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/atfork/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7646 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/atfork/atfork.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1380 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/singleton.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/contrib/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    12903 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/contrib/urlparse25.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      124 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/contrib/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3740 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/json_io.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    27203 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/misc.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    20687 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/algorithms.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7974 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/host.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3836 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    14948 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/reporter.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3683 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/futures.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    14424 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/munch.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10856 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/lockfile.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1770 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/description.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3132 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/get_version.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11057 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugin_manager.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/configs/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      446 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/configs/utils_default.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    18373 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/signatures.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11194 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/url.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4770 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/object_cache.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/plugins/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugins/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1100 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/plugin_unittests_default_2.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1436 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/plugin_unittests_default_1.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1355 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/plugin_unittests_default_2.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1437 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/plugin_unittests_default_1.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    14041 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/lease_manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      321 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     6040 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/testing.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    13494 2021-11-23 16:34:32.000000 radical.utils-1.9.0/src/radical/utils/logger.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10847 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/ids.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11529 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/threads.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9441 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/poll.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5764 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/timing.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    13192 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/dict_mixin.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     6002 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/daemon.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/queue_network/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4337 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/queue_network/network.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      303 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/queue_network/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      735 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/queue_network/node.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      313 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/queue_network/queue.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      936 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/which.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10884 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/registry.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    17498 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/env.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7928 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/heartbeat.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2403 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/modules.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     8900 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/shell.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      195 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/gtod.c
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    13622 2021-11-23 16:34:32.000000 radical.utils-1.9.0/src/radical/utils/config.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1937 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/stack.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    20943 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/debug.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9876 2021-11-23 16:26:24.000000 radical.utils-1.9.0/src/radical/utils/ru_regex.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3374 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/lockable.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    22891 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/flux.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/zmq/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4460 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/bridge.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    16514 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/pubsub.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      468 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5218 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/client.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9200 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/server.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3509 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/registry.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4995 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/utils.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    23063 2021-11-23 17:33:31.000000 radical.utils-1.9.0/src/radical/utils/zmq/queue.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:35:07.000000 radical.utils-1.9.0/src/radical/utils/scheduler/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1953 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/scheduler/scheduler_base.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      197 2021-09-24 08:23:31.000000 radical.utils-1.9.0/src/radical/utils/scheduler/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     8094 2021-11-23 17:33:24.000000 radical.utils-1.9.0/src/radical/utils/scheduler/scheduler_bitarray.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       72 2021-12-14 14:07:27.000000 radical.utils-1.9.1/setup.cfg
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/examples/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/examples/zmq/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/examples/zmq/queue/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      687 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/queue/get.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      662 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/queue/put.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1242 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/queue/queue.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3474 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/protocols.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2290 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/README.md
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/examples/zmq/pubsub/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      575 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/pubsub/pub.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      640 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/pubsub/pubsub.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      598 2021-09-24 08:23:31.000000 radical.utils-1.9.1/examples/zmq/pubsub/sub.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    24901 2021-12-14 14:06:25.000000 radical.utils-1.9.1/CHANGES.md
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9608 2021-12-14 14:05:45.000000 radical.utils-1.9.1/setup.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1210 2021-09-24 08:23:31.000000 radical.utils-1.9.1/README.md
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/bin/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5983 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-utils-mongodb.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      526 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-stack
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      168 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-utils-version
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5247 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-utils-fix-headers.pl
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     7354 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/ru.json.sh
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5581 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-utils-pwatch
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      328 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-utils-pylint.sh
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)    11855 2021-11-23 17:33:31.000000 radical.utils-1.9.1/bin/radical-utils-env.sh
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2695 2021-09-24 08:23:31.000000 radical.utils-1.9.1/bin/radical-bridge
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1285 2021-09-24 08:23:31.000000 radical.utils-1.9.1/LICENSE.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1014 2021-12-14 14:07:27.000000 radical.utils-1.9.1/PKG-INFO
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/test_cases/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4110 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/test_cases/host.00000.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2024 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/test_cases/ids.00000.json
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/bin/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      998 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/bin/ru-runcheck.sh
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/unittests/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4860 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_ids.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3293 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/unittests/test_zmq_client.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3227 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_object_cache.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5016 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/unittests/test_host.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1993 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_json.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2280 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_plugin_manager.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1370 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_regex.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4278 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_lockfile.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/__init__.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3060 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_zmq_pubsub.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4399 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_dict_mixin.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1358 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/unittests/test_zmq_registry.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1258 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_signatures.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1273 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_locks.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9022 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_zmq_queue.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4643 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_algorithms.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/unittests/data/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      469 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/data/import_file.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       99 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/data/resource_yale.json
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      923 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_singleton.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3806 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_lease_manager.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1447 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_poll.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4552 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_logger.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2959 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_read_json.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8610 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_misc.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2311 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_time.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1806 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_daemonize.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1579 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_config.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4573 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_profiler.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2962 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_description.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3571 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_heartbeat.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3354 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_lockable.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      781 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_which.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4006 2021-11-23 16:26:24.000000 radical.utils-1.9.1/tests/unittests/test_env.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2121 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/unittests/test_stack.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     7528 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_url.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3712 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_reporter.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)    10261 2021-12-14 14:05:33.000000 radical.utils-1.9.1/tests/unittests/test_munch.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/tests/integration_tests/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3114 2021-09-24 08:23:31.000000 radical.utils-1.9.1/tests/integration_tests/test_flux.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-12-14 14:06:28.000000 radical.utils-1.9.1/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      107 2021-09-24 08:23:31.000000 radical.utils-1.9.1/MANIFEST.in
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       82 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/top_level.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1014 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4600 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical.utils.egg-info/SOURCES.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    27801 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/profile.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       41 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/SDIST
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3160 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/tracer.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/atfork/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3088 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/atfork/stdlib_fixer.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2022 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/atfork/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7646 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/atfork/atfork.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1380 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/singleton.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/contrib/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12903 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/contrib/urlparse25.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      124 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/contrib/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3740 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/json_io.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    27203 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/misc.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    20687 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/algorithms.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7974 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/host.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3836 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    14948 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/reporter.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3683 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/futures.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    14424 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/munch.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10856 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/lockfile.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1770 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/description.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3132 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/get_version.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11057 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugin_manager.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/configs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      446 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/configs/utils_default.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    18373 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/signatures.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11194 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/url.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4770 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/object_cache.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/plugins/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugins/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1100 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/plugin_unittests_default_2.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1436 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/plugin_unittests_default_1.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1355 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/plugin_unittests_default_2.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1437 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/plugin_unittests_default_1.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    14041 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/lease_manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      321 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     6040 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/testing.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    13494 2021-11-23 16:34:32.000000 radical.utils-1.9.1/src/radical/utils/logger.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10847 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/ids.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11529 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/threads.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9441 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/poll.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5764 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/timing.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    13192 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/dict_mixin.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     6002 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/daemon.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/queue_network/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4337 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/queue_network/network.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      303 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/queue_network/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      735 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/queue_network/node.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      313 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/queue_network/queue.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      936 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/which.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10884 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/registry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    17498 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/env.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7928 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/heartbeat.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2403 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/modules.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     8900 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/shell.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      195 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/gtod.c
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    13622 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/config.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1937 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/stack.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    20943 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/debug.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9876 2021-11-23 16:26:24.000000 radical.utils-1.9.1/src/radical/utils/ru_regex.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3374 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/lockable.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    22891 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/flux.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/zmq/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4460 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/bridge.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    16514 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/pubsub.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      468 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5218 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/client.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9200 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/server.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3509 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/zmq/registry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4995 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/utils.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    23063 2021-12-14 14:05:33.000000 radical.utils-1.9.1/src/radical/utils/zmq/queue.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-12-14 14:07:27.000000 radical.utils-1.9.1/src/radical/utils/scheduler/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1953 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/scheduler/scheduler_base.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      197 2021-09-24 08:23:31.000000 radical.utils-1.9.1/src/radical/utils/scheduler/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     8094 2021-11-23 17:33:24.000000 radical.utils-1.9.1/src/radical/utils/scheduler/scheduler_bitarray.py
```

### Comparing `radical.utils-1.9.0/examples/zmq/queue/get.py` & `radical.utils-1.9.1/examples/zmq/queue/get.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/queue/put.py` & `radical.utils-1.9.1/examples/zmq/queue/put.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/queue/queue.py` & `radical.utils-1.9.1/examples/zmq/queue/queue.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/protocols.md` & `radical.utils-1.9.1/examples/zmq/protocols.md`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/README.md` & `radical.utils-1.9.1/examples/zmq/README.md`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/pubsub/pub.py` & `radical.utils-1.9.1/examples/zmq/pubsub/pub.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/pubsub/pubsub.py` & `radical.utils-1.9.1/examples/zmq/pubsub/pubsub.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/examples/zmq/pubsub/sub.py` & `radical.utils-1.9.1/examples/zmq/pubsub/sub.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/CHANGES.md` & `radical.utils-1.9.1/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 
 For a list of open issues and known problems, see
 https://github.com/radical-cybertools/radical.utils/issues/
 
 
+1.9.1  Hotfix Release                                                 2021-11-23
+--------------------------------------------------------------------------------
+
+  - constrain mongodb version dependency
+
+
 1.9.0  Release                                                        2021-11-23
 --------------------------------------------------------------------------------
 
   - fixed `tarfile` method name
   - generic deactivate
   - pylint fixes, wrap open for utf8 encoding
```

### Comparing `radical.utils-1.9.0/setup.py` & `radical.utils-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     'package_data'       : {'': ['*.txt', '*.sh', '*.json', '*.gz', '*.c',
                                  'VERSION', 'CHANGES.md', 'SDIST', sdist_name]},
   # 'setup_requires'     : ['pytest-runner'],
     'install_requires'   : ['colorama',
                             'msgpack',
                             'netifaces',
                             'ntplib',
-                            'pymongo',
+                            'pymongo<4',
                             'pyzmq',
                             'radical.gtod',
                             'regex',
                             'setproctitle',
                            ],
     'tests_require'      : ['pytest',
                             'pylint',
```

### Comparing `radical.utils-1.9.0/README.md` & `radical.utils-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-utils-mongodb.py` & `radical.utils-1.9.1/bin/radical-utils-mongodb.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-stack` & `radical.utils-1.9.1/bin/radical-stack`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-utils-fix-headers.pl` & `radical.utils-1.9.1/bin/radical-utils-fix-headers.pl`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/ru.json.sh` & `radical.utils-1.9.1/bin/ru.json.sh`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-utils-pwatch` & `radical.utils-1.9.1/bin/radical-utils-pwatch`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-utils-env.sh` & `radical.utils-1.9.1/bin/radical-utils-env.sh`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/bin/radical-bridge` & `radical.utils-1.9.1/bin/radical-bridge`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/LICENSE.md` & `radical.utils-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/PKG-INFO` & `radical.utils-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.utils
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utilities for RADICAL-Cybertools projects
 Home-page: https://www.github.com/radical-cybertools/radical.utils/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.utils-1.9.0/tests/test_cases/host.00000.json` & `radical.utils-1.9.1/tests/test_cases/host.00000.json`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/test_cases/ids.00000.json` & `radical.utils-1.9.1/tests/test_cases/ids.00000.json`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/bin/ru-runcheck.sh` & `radical.utils-1.9.1/tests/bin/ru-runcheck.sh`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_ids.py` & `radical.utils-1.9.1/tests/unittests/test_ids.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_zmq_client.py` & `radical.utils-1.9.1/tests/unittests/test_zmq_client.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_object_cache.py` & `radical.utils-1.9.1/tests/unittests/test_object_cache.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_host.py` & `radical.utils-1.9.1/tests/unittests/test_host.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_json.py` & `radical.utils-1.9.1/tests/unittests/test_json.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_plugin_manager.py` & `radical.utils-1.9.1/tests/unittests/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_regex.py` & `radical.utils-1.9.1/tests/unittests/test_regex.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_lockfile.py` & `radical.utils-1.9.1/tests/unittests/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_zmq_pubsub.py` & `radical.utils-1.9.1/tests/unittests/test_zmq_pubsub.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_dict_mixin.py` & `radical.utils-1.9.1/tests/unittests/test_dict_mixin.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_zmq_registry.py` & `radical.utils-1.9.1/tests/unittests/test_zmq_registry.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_signatures.py` & `radical.utils-1.9.1/tests/unittests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_locks.py` & `radical.utils-1.9.1/tests/unittests/test_locks.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_zmq_queue.py` & `radical.utils-1.9.1/tests/unittests/test_zmq_queue.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_algorithms.py` & `radical.utils-1.9.1/tests/unittests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_singleton.py` & `radical.utils-1.9.1/tests/unittests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_lease_manager.py` & `radical.utils-1.9.1/tests/unittests/test_lease_manager.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_poll.py` & `radical.utils-1.9.1/tests/unittests/test_poll.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_logger.py` & `radical.utils-1.9.1/tests/unittests/test_logger.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_read_json.py` & `radical.utils-1.9.1/tests/unittests/test_read_json.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_misc.py` & `radical.utils-1.9.1/tests/unittests/test_misc.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_time.py` & `radical.utils-1.9.1/tests/unittests/test_time.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_daemonize.py` & `radical.utils-1.9.1/tests/unittests/test_daemonize.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_config.py` & `radical.utils-1.9.1/tests/unittests/test_config.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_profiler.py` & `radical.utils-1.9.1/tests/unittests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_description.py` & `radical.utils-1.9.1/tests/unittests/test_description.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_heartbeat.py` & `radical.utils-1.9.1/tests/unittests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_lockable.py` & `radical.utils-1.9.1/tests/unittests/test_lockable.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_which.py` & `radical.utils-1.9.1/tests/unittests/test_which.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_env.py` & `radical.utils-1.9.1/tests/unittests/test_env.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_stack.py` & `radical.utils-1.9.1/tests/unittests/test_stack.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_url.py` & `radical.utils-1.9.1/tests/unittests/test_url.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_reporter.py` & `radical.utils-1.9.1/tests/unittests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/unittests/test_munch.py` & `radical.utils-1.9.1/tests/unittests/test_munch.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/tests/integration_tests/test_flux.py` & `radical.utils-1.9.1/tests/integration_tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical.utils.egg-info/PKG-INFO` & `radical.utils-1.9.1/src/radical.utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.utils
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utilities for RADICAL-Cybertools projects
 Home-page: https://www.github.com/radical-cybertools/radical.utils/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.utils-1.9.0/src/radical.utils.egg-info/SOURCES.txt` & `radical.utils-1.9.1/src/radical.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/profile.py` & `radical.utils-1.9.1/src/radical/utils/profile.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/tracer.py` & `radical.utils-1.9.1/src/radical/utils/tracer.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/atfork/stdlib_fixer.py` & `radical.utils-1.9.1/src/radical/utils/atfork/stdlib_fixer.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/atfork/__init__.py` & `radical.utils-1.9.1/src/radical/utils/atfork/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/atfork/atfork.py` & `radical.utils-1.9.1/src/radical/utils/atfork/atfork.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/singleton.py` & `radical.utils-1.9.1/src/radical/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/contrib/urlparse25.py` & `radical.utils-1.9.1/src/radical/utils/contrib/urlparse25.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/json_io.py` & `radical.utils-1.9.1/src/radical/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/misc.py` & `radical.utils-1.9.1/src/radical/utils/misc.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/algorithms.py` & `radical.utils-1.9.1/src/radical/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/host.py` & `radical.utils-1.9.1/src/radical/utils/host.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/__init__.py` & `radical.utils-1.9.1/src/radical/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/reporter.py` & `radical.utils-1.9.1/src/radical/utils/reporter.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/futures.py` & `radical.utils-1.9.1/src/radical/utils/futures.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/munch.py` & `radical.utils-1.9.1/src/radical/utils/munch.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/lockfile.py` & `radical.utils-1.9.1/src/radical/utils/lockfile.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/description.py` & `radical.utils-1.9.1/src/radical/utils/description.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/get_version.py` & `radical.utils-1.9.1/src/radical/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/plugin_manager.py` & `radical.utils-1.9.1/src/radical/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/signatures.py` & `radical.utils-1.9.1/src/radical/utils/signatures.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/url.py` & `radical.utils-1.9.1/src/radical/utils/url.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/object_cache.py` & `radical.utils-1.9.1/src/radical/utils/object_cache.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/plugin_unittests_default_2.py` & `radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/plugin_unittests_default_2.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/plugins/unittests_2/plugin_unittests_default_1.py` & `radical.utils-1.9.1/src/radical/utils/plugins/unittests_2/plugin_unittests_default_1.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/plugin_unittests_default_2.py` & `radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/plugin_unittests_default_2.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/plugins/unittests_1/plugin_unittests_default_1.py` & `radical.utils-1.9.1/src/radical/utils/plugins/unittests_1/plugin_unittests_default_1.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/lease_manager.py` & `radical.utils-1.9.1/src/radical/utils/lease_manager.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/testing.py` & `radical.utils-1.9.1/src/radical/utils/testing.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/logger.py` & `radical.utils-1.9.1/src/radical/utils/logger.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/ids.py` & `radical.utils-1.9.1/src/radical/utils/ids.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/threads.py` & `radical.utils-1.9.1/src/radical/utils/threads.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/poll.py` & `radical.utils-1.9.1/src/radical/utils/poll.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/timing.py` & `radical.utils-1.9.1/src/radical/utils/timing.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/dict_mixin.py` & `radical.utils-1.9.1/src/radical/utils/dict_mixin.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/daemon.py` & `radical.utils-1.9.1/src/radical/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/queue_network/network.py` & `radical.utils-1.9.1/src/radical/utils/queue_network/network.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/queue_network/node.py` & `radical.utils-1.9.1/src/radical/utils/queue_network/node.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/which.py` & `radical.utils-1.9.1/src/radical/utils/which.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/registry.py` & `radical.utils-1.9.1/src/radical/utils/registry.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/env.py` & `radical.utils-1.9.1/src/radical/utils/env.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/heartbeat.py` & `radical.utils-1.9.1/src/radical/utils/heartbeat.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/modules.py` & `radical.utils-1.9.1/src/radical/utils/modules.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/shell.py` & `radical.utils-1.9.1/src/radical/utils/shell.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/config.py` & `radical.utils-1.9.1/src/radical/utils/config.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/stack.py` & `radical.utils-1.9.1/src/radical/utils/stack.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/debug.py` & `radical.utils-1.9.1/src/radical/utils/debug.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/ru_regex.py` & `radical.utils-1.9.1/src/radical/utils/ru_regex.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/lockable.py` & `radical.utils-1.9.1/src/radical/utils/lockable.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/flux.py` & `radical.utils-1.9.1/src/radical/utils/flux.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/bridge.py` & `radical.utils-1.9.1/src/radical/utils/zmq/bridge.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/pubsub.py` & `radical.utils-1.9.1/src/radical/utils/zmq/pubsub.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/client.py` & `radical.utils-1.9.1/src/radical/utils/zmq/client.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/server.py` & `radical.utils-1.9.1/src/radical/utils/zmq/server.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/registry.py` & `radical.utils-1.9.1/src/radical/utils/zmq/registry.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/utils.py` & `radical.utils-1.9.1/src/radical/utils/zmq/utils.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/zmq/queue.py` & `radical.utils-1.9.1/src/radical/utils/zmq/queue.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/scheduler/scheduler_base.py` & `radical.utils-1.9.1/src/radical/utils/scheduler/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `radical.utils-1.9.0/src/radical/utils/scheduler/scheduler_bitarray.py` & `radical.utils-1.9.1/src/radical/utils/scheduler/scheduler_bitarray.py`

 * *Files identical despite different names*

