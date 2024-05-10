# Comparing `tmp/fcio-0.4.0.dev5.tar.gz` & `tmp/fcio-0.4.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcio-0.4.0.dev5.tar", last modified: Thu May  9 12:28:39 2024, max compression
+gzip compressed data, was "fcio-0.4.0.dev6.tar", last modified: Thu May  9 12:35:27 2024, max compression
```

## Comparing `fcio-0.4.0.dev5.tar` & `fcio-0.4.0.dev6.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     1597 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/.github/workflows/gh-pages-static.yml
--rw-r--r--   0        0        0     1720 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/.github/workflows/main.yml
--rw-r--r--   0        0        0     3178 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/.github/workflows/publish.yml
--rw-r--r--   0        0        0       51 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/.gitignore
--rw-r--r--   0        0        0      761 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/CHANGELOG.md
--rw-r--r--   0        0        0    16726 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/LICENSE
--rw-r--r--   0        0        0      628 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/Makefile
--rw-r--r--   0        0        0     1961 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/README.md
--rw-r--r--   0        0        0      638 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/Makefile
--rw-r--r--   0        0        0      804 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/make.bat
--rw-r--r--   0        0        0       29 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/requirements.txt
--rw-r--r--   0        0        0     1729 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/source/conf.py
--rw-r--r--   0        0        0      238 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/source/fcio.rst
--rw-r--r--   0        0        0      223 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/source/index.rst
--rw-r--r--   0        0        0       45 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/docs/source/readme.rst
--rw-r--r--   0        0        0     1200 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/meson.build
--rw-r--r--   0        0        0     2178 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/pyproject.toml
--rw-r--r--   0        0        0      714 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/__init__.py
--rw-r--r--   0        0        0       92 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cmds/__init__.py
--rw-r--r--   0        0        0     3071 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cmds/cmds.py
--rw-r--r--   0        0        0     1943 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cppyy_fcio/config.py
--rw-r--r--   0        0        0     8387 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cppyy_fcio/event.py
--rw-r--r--   0        0        0     4344 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cppyy_fcio/fcio_cppyy.py
--rw-r--r--   0        0        0     2957 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cppyy_fcio/status.py
--rw-r--r--   0        0        0     4591 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cfcio.pxd
--rw-r--r--   0        0        0     3646 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_dead_interval_tracker.pyx
--rw-r--r--   0        0        0    10806 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio.pyx
--rw-r--r--   0        0        0     3742 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_config.pyx
--rw-r--r--   0        0        0     5827 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_event.pyx
--rw-r--r--   0        0        0     8541 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
--rw-r--r--   0        0        0     4896 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_recevent.pyx
--rw-r--r--   0        0        0     7503 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx
--rw-r--r--   0        0        0     6425 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_status.pyx
--rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/.drone.star
--rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/.gitignore
--rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/LICENSE
--rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/Makefile
--rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/README.md
--rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/examples/bufio_benchmark.c
--rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/examples/meson.build
--rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/meson.build
--rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/src/bufio.c
--rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/src/bufio.h
--rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/src/meson.build
--rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
--rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_follow.c
--rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_follow_chunk.c
--rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_lockedfile.c
--rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_tcp_connect.c
--rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
--rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
--rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/meson.build
--rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.4.0.dev5/subprojects/bufio/tests/test.h
--rw-r--r--   0        0        0      110 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/subprojects/bufio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/.drone.star
--rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/LICENSE
--rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/Makefile
--rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/README.md
--rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/meson.build
--rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/src/fcio.c
--rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/src/fcio.h
--rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/src/meson.build
--rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/src/time_utils.c
--rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/src/time_utils.h
--rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.4.0.dev5/subprojects/fcio/subprojects/tmio.wrap
--rw-r--r--   0        0        0      109 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/subprojects/fcio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/.drone.star
--rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/LICENSE
--rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/Makefile
--rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/README.md
--rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/meson.build
--rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/timer.c
--rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/timer.h
--rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark.c
--rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
--rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
--rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_pipe.sh
--rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_simple.c
--rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_tcp.sh
--rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_example_reader.c
--rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_example_writer.c
--rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_sink.c
--rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/meson.build
--rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/src/meson.build
--rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/src/tmio.c
--rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/src/tmio.h
--rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.4.0.dev5/subprojects/tmio/subprojects/bufio.wrap
--rw-r--r--   0        0        0      108 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/subprojects/tmio.wrap
--rwxr-xr-x   0        0        0     1358 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/tests/test_integration.py
--rwxr-xr-x   0        0        0      526 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/tests/test_platform.py
--rwxr-xr-x   0        0        0      249 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/tools/create-pxd.sh
--rwxr-xr-x   0        0        0     1374 2024-05-09 12:27:07.000000 fcio-0.4.0.dev5/tools/version_util.py
--rw-r--r--   0        0        0     3386 2024-05-09 12:28:39.661502 fcio-0.4.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/.github/workflows/gh-pages-static.yml
+-rw-r--r--   0        0        0     1720 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3178 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       51 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/.gitignore
+-rw-r--r--   0        0        0      761 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/CHANGELOG.md
+-rw-r--r--   0        0        0    16726 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/Makefile
+-rw-r--r--   0        0        0     1961 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/README.md
+-rw-r--r--   0        0        0      638 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/make.bat
+-rw-r--r--   0        0        0       29 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/requirements.txt
+-rw-r--r--   0        0        0     1729 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/source/conf.py
+-rw-r--r--   0        0        0      238 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/source/fcio.rst
+-rw-r--r--   0        0        0      223 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/source/index.rst
+-rw-r--r--   0        0        0       45 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/docs/source/readme.rst
+-rw-r--r--   0        0        0     1200 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/meson.build
+-rw-r--r--   0        0        0     2178 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cmds/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cmds/cmds.py
+-rw-r--r--   0        0        0     1943 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cppyy_fcio/config.py
+-rw-r--r--   0        0        0     8387 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cppyy_fcio/event.py
+-rw-r--r--   0        0        0     4344 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cppyy_fcio/fcio_cppyy.py
+-rw-r--r--   0        0        0     2957 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cppyy_fcio/status.py
+-rw-r--r--   0        0        0     4591 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cfcio.pxd
+-rw-r--r--   0        0        0     3646 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_dead_interval_tracker.pyx
+-rw-r--r--   0        0        0    10806 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio.pyx
+-rw-r--r--   0        0        0     3742 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_config.pyx
+-rw-r--r--   0        0        0     5827 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_event.pyx
+-rw-r--r--   0        0        0     8541 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
+-rw-r--r--   0        0        0     4896 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_recevent.pyx
+-rw-r--r--   0        0        0     7503 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx
+-rw-r--r--   0        0        0     6425 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_status.pyx
+-rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/.drone.star
+-rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/LICENSE
+-rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/Makefile
+-rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/README.md
+-rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/examples/bufio_benchmark.c
+-rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/examples/meson.build
+-rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/meson.build
+-rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/src/bufio.c
+-rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/src/bufio.h
+-rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/src/meson.build
+-rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
+-rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_follow.c
+-rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_follow_chunk.c
+-rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_lockedfile.c
+-rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_tcp_connect.c
+-rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
+-rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
+-rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/meson.build
+-rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.4.0.dev6/subprojects/bufio/tests/test.h
+-rw-r--r--   0        0        0      110 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/.drone.star
+-rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/LICENSE
+-rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/Makefile
+-rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/README.md
+-rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/meson.build
+-rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/src/fcio.c
+-rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/src/fcio.h
+-rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/src/meson.build
+-rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/src/time_utils.c
+-rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/src/time_utils.h
+-rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.4.0.dev6/subprojects/fcio/subprojects/tmio.wrap
+-rw-r--r--   0        0        0      109 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/subprojects/fcio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/.drone.star
+-rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/LICENSE
+-rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/Makefile
+-rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/README.md
+-rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/meson.build
+-rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/timer.c
+-rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/timer.h
+-rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark.c
+-rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
+-rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
+-rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_pipe.sh
+-rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_simple.c
+-rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_tcp.sh
+-rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_example_reader.c
+-rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_example_writer.c
+-rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_sink.c
+-rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/meson.build
+-rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/src/meson.build
+-rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/src/tmio.c
+-rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/src/tmio.h
+-rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.4.0.dev6/subprojects/tmio/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      108 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/subprojects/tmio.wrap
+-rwxr-xr-x   0        0        0     1358 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/tests/test_integration.py
+-rwxr-xr-x   0        0        0      526 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/tests/test_platform.py
+-rwxr-xr-x   0        0        0      249 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/tools/create-pxd.sh
+-rwxr-xr-x   0        0        0     1374 2024-05-09 12:34:04.000000 fcio-0.4.0.dev6/tools/version_util.py
+-rw-r--r--   0        0        0     3386 2024-05-09 12:35:27.783953 fcio-0.4.0.dev6/PKG-INFO
```

### Comparing `fcio-0.4.0.dev5/.github/workflows/gh-pages-static.yml` & `fcio-0.4.0.dev6/.github/workflows/gh-pages-static.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     steps:
       - name: Render
         run: |
-          ls ${{ github.workspace }}/fcio-py
-          cd ${{ github.workspace }}/fcio-py
           python -m pip install -U pip
           python -m pip install -r docs/requirements.txt
           python -m pip install fcio
           sphinx-apidoc --force --no-toc --no-headings --output docs/source .
           sphinx-build -M html docs/source/ docs/build/
       - name: Setup Pages
         uses: actions/configure-pages@v3
```

### Comparing `fcio-0.4.0.dev5/.github/workflows/main.yml` & `fcio-0.4.0.dev6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/.github/workflows/publish.yml` & `fcio-0.4.0.dev6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/CHANGELOG.md` & `fcio-0.4.0.dev6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/LICENSE` & `fcio-0.4.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/Makefile` & `fcio-0.4.0.dev6/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/README.md` & `fcio-0.4.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/docs/Makefile` & `fcio-0.4.0.dev6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/docs/make.bat` & `fcio-0.4.0.dev6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/docs/source/conf.py` & `fcio-0.4.0.dev6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/meson.build` & `fcio-0.4.0.dev6/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/pyproject.toml` & `fcio-0.4.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/__init__.py` & `fcio-0.4.0.dev6/src/fcio/__init__.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cmds/cmds.py` & `fcio-0.4.0.dev6/src/fcio/cmds/cmds.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cppyy_fcio/config.py` & `fcio-0.4.0.dev6/src/fcio/cppyy_fcio/config.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cppyy_fcio/event.py` & `fcio-0.4.0.dev6/src/fcio/cppyy_fcio/event.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cppyy_fcio/fcio_cppyy.py` & `fcio-0.4.0.dev6/src/fcio/cppyy_fcio/fcio_cppyy.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cppyy_fcio/status.py` & `fcio-0.4.0.dev6/src/fcio/cppyy_fcio/status.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cfcio.pxd` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cfcio.pxd`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_dead_interval_tracker.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_dead_interval_tracker.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_config.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_config.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_event.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_event.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_event_ext.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_event_ext.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_recevent.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_recevent.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/src/fcio/cy_fcio/cy_fcio_status.pyx` & `fcio-0.4.0.dev6/src/fcio/cy_fcio/cy_fcio_status.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/.drone.star` & `fcio-0.4.0.dev6/subprojects/bufio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/LICENSE` & `fcio-0.4.0.dev6/subprojects/bufio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/examples/bufio_benchmark.c` & `fcio-0.4.0.dev6/subprojects/bufio/examples/bufio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/meson.build` & `fcio-0.4.0.dev6/subprojects/bufio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/src/bufio.c` & `fcio-0.4.0.dev6/subprojects/bufio/src/bufio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/src/bufio.h` & `fcio-0.4.0.dev6/subprojects/bufio/src/bufio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_follow.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_follow.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_follow_chunk.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_follow_chunk.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_lockedfile.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_lockedfile.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_tcp_connect.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c` & `fcio-0.4.0.dev6/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/bufio/tests/meson.build` & `fcio-0.4.0.dev6/subprojects/bufio/tests/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/.drone.star` & `fcio-0.4.0.dev6/subprojects/fcio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/LICENSE` & `fcio-0.4.0.dev6/subprojects/fcio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/README.md` & `fcio-0.4.0.dev6/subprojects/fcio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/meson.build` & `fcio-0.4.0.dev6/subprojects/fcio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/src/fcio.c` & `fcio-0.4.0.dev6/subprojects/fcio/src/fcio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/src/fcio.h` & `fcio-0.4.0.dev6/subprojects/fcio/src/fcio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/src/time_utils.c` & `fcio-0.4.0.dev6/subprojects/fcio/src/time_utils.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/fcio/src/time_utils.h` & `fcio-0.4.0.dev6/subprojects/fcio/src/time_utils.h`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/.drone.star` & `fcio-0.4.0.dev6/subprojects/tmio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/LICENSE` & `fcio-0.4.0.dev6/subprojects/tmio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/README.md` & `fcio-0.4.0.dev6/subprojects/tmio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/meson.build` & `fcio-0.4.0.dev6/subprojects/tmio/examples/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/timer.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/timer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/timer.h` & `fcio-0.4.0.dev6/subprojects/tmio/examples/timer.h`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_disk_read.sh` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_disk_read.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_disk_write.sh` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_disk_write.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_pipe.sh` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_pipe.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_simple.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_simple.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_benchmark_tcp.sh` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_benchmark_tcp.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_example_reader.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_example_reader.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_example_writer.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_example_writer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/examples/tmio_sink.c` & `fcio-0.4.0.dev6/subprojects/tmio/examples/tmio_sink.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/meson.build` & `fcio-0.4.0.dev6/subprojects/tmio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/src/tmio.c` & `fcio-0.4.0.dev6/subprojects/tmio/src/tmio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/subprojects/tmio/src/tmio.h` & `fcio-0.4.0.dev6/subprojects/tmio/src/tmio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/tests/test_integration.py` & `fcio-0.4.0.dev6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/tests/test_platform.py` & `fcio-0.4.0.dev6/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/tools/version_util.py` & `fcio-0.4.0.dev6/tools/version_util.py`

 * *Files identical despite different names*

### Comparing `fcio-0.4.0.dev5/PKG-INFO` & `fcio-0.4.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcio
-Version: 0.4.0.dev5
+Version: 0.4.0.dev6
 Summary: FlashCam File Format (FCIO) reader for python.
 Author-Email: Simon Sailer <simon.sailer@mpi-hd.mpg.de>
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

