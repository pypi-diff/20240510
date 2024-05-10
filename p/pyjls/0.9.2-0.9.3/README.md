# Comparing `tmp/pyjls-0.9.2.tar.gz` & `tmp/pyjls-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.9.2.tar", last modified: Wed Feb 14 16:29:53 2024, max compression
+gzip compressed data, was "pyjls-0.9.3.tar", last modified: Thu Mar  7 19:33:42 2024, max compression
```

## Comparing `pyjls-0.9.2.tar` & `pyjls-0.9.3.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.692505 pyjls-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-02-14 16:29:40.000000 pyjls-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-14 16:29:40.000000 pyjls-0.9.2/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-14 16:29:40.000000 pyjls-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-14 16:29:40.000000 pyjls-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-02-14 16:29:53.692505 pyjls-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-02-14 16:29:40.000000 pyjls-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.680505 pyjls-0.9.2/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.680505 pyjls-0.9.2/include/jls/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/backend.h
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/cmacro.h
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/copy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/crc32c.h
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/ec.h
--rw-r--r--   0 runner    (1001) docker     (127)    24438 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/format.h
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/log.h
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/raw.h
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/reader.h
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/statistics.h
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/threaded_writer.h
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/time.h
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/version.h
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls/writer.h
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-14 16:29:40.000000 pyjls-0.9.2/include/jls.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.676505 pyjls-0.9.2/include_prv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.684505 pyjls-0.9.2/include_prv/jls/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/bit_shift.h
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/cdef.h
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/core.h
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/datatype.h
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/msg_ring_buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/tmap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/track.h
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/wr_fsr.h
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/wr_prv.h
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-14 16:29:40.000000 pyjls-0.9.2/include_prv/jls/wr_ts.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.684505 pyjls-0.9.2/pyjls/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2170889 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.688505 pyjls-0.9.2/pyjls/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/entry_points/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.688505 pyjls-0.9.2/pyjls/test/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/test/test_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.688505 pyjls-0.9.2/pyjls/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyjls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.692505 pyjls-0.9.2/pyjls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 16:29:53.000000 pyjls-0.9.2/pyjls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-14 16:29:40.000000 pyjls-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 16:29:53.692505 pyjls-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-02-14 16:29:40.000000 pyjls-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:29:53.692505 pyjls-0.9.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/backend_posix.c
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/backend_win.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/bit_shift.c
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/copy.c
--rw-r--r--   0 runner    (1001) docker     (127)    53447 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/crc32c.c
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/crc32c_arm_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/crc32c_intel_sse4.c
--rw-r--r--   0 runner    (1001) docker     (127)    33131 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/crc32c_sw.c
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/datatype.c
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/ec.c
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/log.c
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/msg_ring_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/raw.c
--rw-r--r--   0 runner    (1001) docker     (127)    27970 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/reader.c
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/statistics.c
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/threaded_writer.c
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/tmap.c
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/track.c
--rw-r--r--   0 runner    (1001) docker     (127)    24972 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/wr_fsr.c
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/wr_ts.c
--rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-02-14 16:29:40.000000 pyjls-0.9.2/src/writer.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.678057 pyjls-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-03-07 19:33:33.000000 pyjls-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-07 19:33:33.000000 pyjls-0.9.3/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 19:33:33.000000 pyjls-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-07 19:33:33.000000 pyjls-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-03-07 19:33:42.678057 pyjls-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-03-07 19:33:33.000000 pyjls-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.662057 pyjls-0.9.3/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.666056 pyjls-0.9.3/include/jls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/backend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/cmacro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/copy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/crc32c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/ec.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24438 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/format.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/raw.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/statistics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/threaded_writer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/time.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls/writer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-07 19:33:33.000000 pyjls-0.9.3/include/jls.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.662057 pyjls-0.9.3/include_prv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.666056 pyjls-0.9.3/include_prv/jls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/bit_shift.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/cdef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/datatype.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/msg_ring_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/tmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/track.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/wr_fsr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/wr_prv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-07 19:33:33.000000 pyjls-0.9.3/include_prv/jls/wr_ts.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.670057 pyjls-0.9.3/pyjls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2170540 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.670057 pyjls-0.9.3/pyjls/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/entry_points/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.670057 pyjls-0.9.3/pyjls/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/test/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/time64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.674057 pyjls-0.9.3/pyjls/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyjls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.678057 pyjls-0.9.3/pyjls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 19:33:42.000000 pyjls-0.9.3/pyjls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-07 19:33:33.000000 pyjls-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 19:33:42.678057 pyjls-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-07 19:33:33.000000 pyjls-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 19:33:42.678057 pyjls-0.9.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/backend_posix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/backend_win.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/bit_shift.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/copy.c
+-rw-r--r--   0 runner    (1001) docker     (127)    53447 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/crc32c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/crc32c_arm_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/crc32c_intel_sse4.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33131 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/crc32c_sw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/datatype.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/ec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/msg_ring_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/raw.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27970 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/reader.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/statistics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/threaded_writer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/tmap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/track.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24972 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/wr_fsr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/wr_ts.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-03-07 19:33:33.000000 pyjls-0.9.3/src/writer.c
```

### Comparing `pyjls-0.9.2/CHANGELOG.md` & `pyjls-0.9.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.9.3
+
+2024 Mar 7
+
+* Added "export" python subcommand.
+
+
 ## 0.9.2
 
 2024 Feb 14
 
 * Fixed index error in file repair operation.
 * Fixed FSR summary reconstruction on truncation  #10
```

### Comparing `pyjls-0.9.2/CREDITS.html` & `pyjls-0.9.3/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/LICENSE` & `pyjls-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/PKG-INFO` & `pyjls-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.9.2
+Version: 0.9.3
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.9.2/README.md` & `pyjls-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/backend.h` & `pyjls-0.9.3/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/cmacro.h` & `pyjls-0.9.3/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/copy.h` & `pyjls-0.9.3/include/jls/copy.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/crc32c.h` & `pyjls-0.9.3/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/ec.h` & `pyjls-0.9.3/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/format.h` & `pyjls-0.9.3/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/log.h` & `pyjls-0.9.3/include/jls/log.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/raw.h` & `pyjls-0.9.3/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/reader.h` & `pyjls-0.9.3/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/statistics.h` & `pyjls-0.9.3/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/threaded_writer.h` & `pyjls-0.9.3/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/time.h` & `pyjls-0.9.3/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls/version.h` & `pyjls-0.9.3/include/jls/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
 #define JLS_VERSION_MINOR 9
-#define JLS_VERSION_PATCH 2
+#define JLS_VERSION_PATCH 3
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.9.2/include/jls/writer.h` & `pyjls-0.9.3/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include/jls.h` & `pyjls-0.9.3/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/bit_shift.h` & `pyjls-0.9.3/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/buffer.h` & `pyjls-0.9.3/include_prv/jls/buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/cdef.h` & `pyjls-0.9.3/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/core.h` & `pyjls-0.9.3/include_prv/jls/core.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/datatype.h` & `pyjls-0.9.3/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.9.3/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/tmap.h` & `pyjls-0.9.3/include_prv/jls/tmap.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/track.h` & `pyjls-0.9.3/include_prv/jls/track.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/util.h` & `pyjls-0.9.3/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/wr_fsr.h` & `pyjls-0.9.3/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/wr_prv.h` & `pyjls-0.9.3/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/include_prv/jls/wr_ts.h` & `pyjls-0.9.3/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/__init__.py` & `pyjls-0.9.3/pyjls/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 # limitations under the License.
 
 from .binding import DataType, AnnotationType, SignalType, Writer, Reader, SummaryFSR, \
     copy, \
     data_type_as_enum, data_type_as_str, \
     utc_to_jls, jls_to_utc
 from .structs import SourceDef, SignalDef
+from . import time64
 from .version import *
 
 __all__ = ['Writer', 'Reader', 'DataType', 'AnnotationType',
            'SignalType', 'SourceDef', 'SignalDef', 'SummaryFSR',
            'copy',
            'data_type_as_enum', 'data_type_as_str',
            'utc_to_jls', 'jls_to_utc',
+           'time64',
            '__version__', '__title__', '__description__', '__url__',
            '__author__', '__author_email__', '__license__',
            '__copyright__']
```

### Comparing `pyjls-0.9.2/pyjls/__main__.py` & `pyjls-0.9.3/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/binding.c` & `pyjls-0.9.3/pyjls/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.9 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-msse4.2"
         ],
         "include_dirs": [
             "include",
             "include_prv",
-            "/tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/core/include"
         ],
         "libraries": [
             "pthread",
             "m"
         ],
         "name": "pyjls.binding",
         "sources": [
@@ -70,18 +70,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x030009F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -766,16 +766,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1119,15 +1124,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1206,15 +1211,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1331,32 +1336,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1688,177 +1676,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1894,42 +1882,42 @@
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback;
 struct __pyx_obj_5pyjls_7binding_Reader;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2856,30 +2844,30 @@
 
 /* MergeVTables.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_MergeVtables(PyTypeObject *type);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
+#define __PYX_HAVE_RT_ImportType_proto_3_0_9
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_9 {
+   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -20240,261 +20228,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20503,29 +20491,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20536,15 +20524,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20553,29 +20541,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20586,15 +20574,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20603,29 +20591,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20636,15 +20624,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20653,29 +20641,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20686,15 +20674,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20703,29 +20691,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20736,217 +20724,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -20962,15 +20950,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -20978,68 +20966,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21047,15 +21035,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -21070,15 +21058,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21094,15 +21082,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21110,68 +21098,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21179,15 +21167,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21202,15 +21190,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21226,15 +21214,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21242,68 +21230,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21311,15 +21299,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21334,170 +21322,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -38093,26 +38081,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-14sdrr08/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-42bma0fd/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -39059,41 +39047,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -46320,18 +46308,18 @@
     __Pyx_DECREF_TypeName(base_name);
     free(base_vtables);
     return -1;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_9
+#define __PYX_HAVE_RT_ImportType_3_0_9
+static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -46377,23 +46365,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -47385,15 +47373,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `pyjls-0.9.2/pyjls/entry_points/__init__.py` & `pyjls-0.9.3/pyjls/entry_points/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import annotate, copy, export, info, plot
+from . import annotate, copy, export, extract, info, plot
 
-__all__ = [annotate, copy, export, info, plot]
+__all__ = [annotate, copy, export, extract, info, plot]
 """This list of available command modules.  Each module must contain a 
 parser_config(subparser) function.  The function must return the callable(args)
 that will be executed for the command."""
```

### Comparing `pyjls-0.9.2/pyjls/entry_points/annotate.py` & `pyjls-0.9.3/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/entry_points/copy.py` & `pyjls-0.9.3/pyjls/entry_points/copy.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     msg = f'[{bar}] {percents:3d}% {message:40s}\r'
     sys.stdout.write(msg)
     sys.stdout.flush()
 
 
 def parser_config(p):
-    """Plot JLS file data contents for FSR signals."""
+    """Copy a JLS file by replaying the data.  May recover corrupted files."""
     p.add_argument('src',
                    help='JLS input filename')
     p.add_argument('dst',
                    help='JLS output filename')
     p.add_argument('--no-progress',
                    action='store_true',
                    help='Hide progress bar.')
```

### Comparing `pyjls-0.9.2/pyjls/entry_points/export.py` & `pyjls-0.9.3/pyjls/entry_points/export.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/entry_points/info.py` & `pyjls-0.9.3/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/entry_points/plot.py` & `pyjls-0.9.3/pyjls/entry_points/plot.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/structs.py` & `pyjls-0.9.3/pyjls/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     utc_decimate_factor: int = 0
     sample_id_offset: int = 0
     name: str = None
     units: str = None
     length: int = 0
 
     def info(self, verbose=None) -> str:
-        hdr = f'{self.signal_id}: {self.name}'
+        hdr = f'{self.signal_id}: {self.source_id}.{self.name}'
         if self.signal_type == 0:
             hdr += f' ({self.length} samples at {self.sample_rate} Hz)'
         strs = [hdr]
         if verbose:
             for field in ['source_id', 'signal_type', 'data_type', 'sample_rate',
                           'samples_per_data', 'sample_decimate_factor',
                           'entries_per_summary', 'summary_decimate_factor',
```

### Comparing `pyjls-0.9.2/pyjls/test/__init__.py` & `pyjls-0.9.3/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/test/test_binding.py` & `pyjls-0.9.3/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/v1/__init__.py` & `pyjls-0.9.3/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/pyjls/version.py` & `pyjls-0.9.3/pyjls/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __title__ = "pyjls"
 __description__ = 'Joulescope™ file format'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjls-0.9.2/pyjls.egg-info/PKG-INFO` & `pyjls-0.9.3/pyjls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.9.2
+Version: 0.9.3
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.9.2/pyjls.egg-info/SOURCES.txt` & `pyjls-0.9.3/pyjls.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,25 +32,27 @@
 include_prv/jls/wr_fsr.h
 include_prv/jls/wr_prv.h
 include_prv/jls/wr_ts.h
 pyjls/__init__.py
 pyjls/__main__.py
 pyjls/binding.c
 pyjls/structs.py
+pyjls/time64.py
 pyjls/version.py
 pyjls.egg-info/PKG-INFO
 pyjls.egg-info/SOURCES.txt
 pyjls.egg-info/dependency_links.txt
 pyjls.egg-info/entry_points.txt
 pyjls.egg-info/requires.txt
 pyjls.egg-info/top_level.txt
 pyjls/entry_points/__init__.py
 pyjls/entry_points/annotate.py
 pyjls/entry_points/copy.py
 pyjls/entry_points/export.py
+pyjls/entry_points/extract.py
 pyjls/entry_points/info.py
 pyjls/entry_points/plot.py
 pyjls/test/__init__.py
 pyjls/test/test_binding.py
 pyjls/v1/__init__.py
 src/backend_posix.c
 src/backend_win.c
```

### Comparing `pyjls-0.9.2/pyproject.toml` & `pyjls-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/setup.py` & `pyjls-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/backend_posix.c` & `pyjls-0.9.3/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/backend_win.c` & `pyjls-0.9.3/src/backend_win.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/bit_shift.c` & `pyjls-0.9.3/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/buffer.c` & `pyjls-0.9.3/src/buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/copy.c` & `pyjls-0.9.3/src/copy.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/core.c` & `pyjls-0.9.3/src/core.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/crc32c.c` & `pyjls-0.9.3/src/crc32c.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/crc32c_arm_neon.c` & `pyjls-0.9.3/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/crc32c_intel_sse4.c` & `pyjls-0.9.3/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/crc32c_sw.c` & `pyjls-0.9.3/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/datatype.c` & `pyjls-0.9.3/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/ec.c` & `pyjls-0.9.3/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/log.c` & `pyjls-0.9.3/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/msg_ring_buffer.c` & `pyjls-0.9.3/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/raw.c` & `pyjls-0.9.3/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/reader.c` & `pyjls-0.9.3/src/reader.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/statistics.c` & `pyjls-0.9.3/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/threaded_writer.c` & `pyjls-0.9.3/src/threaded_writer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/tmap.c` & `pyjls-0.9.3/src/tmap.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/track.c` & `pyjls-0.9.3/src/track.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/wr_fsr.c` & `pyjls-0.9.3/src/wr_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/wr_ts.c` & `pyjls-0.9.3/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.9.2/src/writer.c` & `pyjls-0.9.3/src/writer.c`

 * *Files identical despite different names*

