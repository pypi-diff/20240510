# Comparing `tmp/libvmdk-python-20240303.tar.gz` & `tmp/libvmdk-python-20240510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvmdk-python-20240303.tar", last modified: Sun Mar  3 08:52:05 2024, max compression
+gzip compressed data, was "libvmdk-python-20240510.tar", last modified: Fri May 10 04:46:40 2024, max compression
```

## Comparing `libvmdk-python-20240303.tar` & `libvmdk-python-20240510.tar`

### file list

```diff
@@ -1,836 +1,836 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32730 2024-03-03 08:33:35.000000 libvmdk-20240303/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-03 08:33:18.000000 libvmdk-20240303/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3315 2024-03-03 08:03:11.000000 libvmdk-20240303/libvmdk.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-03 08:03:11.000000 libvmdk-20240303/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-03 08:33:34.000000 libvmdk-20240303/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:03:11.000000 libvmdk-20240303/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-03 08:33:35.000000 libvmdk-20240303/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-03 08:33:28.000000 libvmdk-20240303/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-03 08:33:28.000000 libvmdk-20240303/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-03 08:33:28.000000 libvmdk-20240303/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-03 08:33:28.000000 libvmdk-20240303/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-03 08:33:28.000000 libvmdk-20240303/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:15:30.000000 libvmdk-20240303/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7383 2023-12-03 09:15:29.000000 libvmdk-20240303/m4/zlib.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15626 2024-03-03 08:33:47.000000 libvmdk-20240303/include/libvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-03-03 08:03:11.000000 libvmdk-20240303/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15626 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27472 2024-03-03 08:33:34.000000 libvmdk-20240303/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/include/libvmdk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3321 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3319 2024-03-03 08:33:47.000000 libvmdk-20240303/include/libvmdk/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4981 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2024-03-03 08:33:47.000000 libvmdk-20240303/include/libvmdk/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-03-03 08:33:47.000000 libvmdk-20240303/include/libvmdk/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-03-03 08:03:12.000000 libvmdk-20240303/include/libvmdk/codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-03 08:03:12.000000 libvmdk-20240303/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-03 08:03:12.000000 libvmdk-20240303/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-03 08:03:12.000000 libvmdk-20240303/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-03 08:03:12.000000 libvmdk-20240303/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-03 08:03:12.000000 libvmdk-20240303/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-03 08:03:12.000000 libvmdk-20240303/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-03 08:03:12.000000 libvmdk-20240303/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-03 08:03:11.000000 libvmdk-20240303/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-03 08:03:12.000000 libvmdk-20240303/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-03-03 08:33:47.000000 libvmdk-20240303/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16488 2024-03-03 08:33:34.000000 libvmdk-20240303/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17463 2024-03-03 08:33:47.000000 libvmdk-20240303/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-03 08:03:12.000000 libvmdk-20240303/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-03 08:03:12.000000 libvmdk-20240303/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-03 08:03:12.000000 libvmdk-20240303/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24498 2024-03-03 08:33:34.000000 libvmdk-20240303/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29501 2024-03-03 08:33:35.000000 libvmdk-20240303/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-03 08:33:11.000000 libvmdk-20240303/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/vmdktools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1759 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/vmdkinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18958 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-12-03 09:15:27.000000 libvmdk-20240303/vmdktools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20750 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20587 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15491 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/vmdkmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2702 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26617 2024-03-03 08:04:12.000000 libvmdk-20240303/vmdktools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-03-03 08:33:35.000000 libvmdk-20240303/vmdktools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4031 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/vmdktools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-03-03 08:03:13.000000 libvmdk-20240303/vmdktools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29974 2024-03-03 08:33:35.000000 libvmdk-20240303/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-03 08:33:17.000000 libvmdk-20240303/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2409 2024-03-03 08:33:47.000000 libvmdk-20240303/libvmdk.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2209 2023-12-03 09:15:14.000000 libvmdk-20240303/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32960 2024-03-03 08:33:34.000000 libvmdk-20240303/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-03 08:33:05.000000 libvmdk-20240303/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:15.000000 libvmdk-20240303/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-03 08:33:34.000000 libvmdk-20240303/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-03-03 08:03:14.000000 libvmdk-20240303/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2106 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/libvmdk.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-03-03 08:33:47.000000 libvmdk-20240303/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/libvmdk-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/libvmdk-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-03 08:03:11.000000 libvmdk-20240303/dpkg/libvmdk-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-03-03 08:33:47.000000 libvmdk-20240303/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-03 08:03:11.000000 libvmdk-20240303/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1836195 2024-03-03 08:33:33.000000 libvmdk-20240303/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-03 08:33:34.000000 libvmdk-20240303/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-03 08:33:34.000000 libvmdk-20240303/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/pyvmdk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13199 2024-03-03 08:04:12.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_libvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_disk_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_file_objects_io_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1324 2023-12-03 09:15:28.000000 libvmdk-20240303/pyvmdk/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_file_objects_io_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10226 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_disk_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2590 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptors.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4736 2024-03-03 08:04:12.000000 libvmdk-20240303/pyvmdk/pyvmdk_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1631 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9785 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptors.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-03 08:03:13.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1851 2024-03-03 08:04:12.000000 libvmdk-20240303/pyvmdk/pyvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2529 2024-03-03 08:04:12.000000 libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46841 2024-03-03 08:33:35.000000 libvmdk-20240303/pyvmdk/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16068 2024-03-03 08:04:12.000000 libvmdk-20240303/pyvmdk/pyvmdk.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45944 2024-03-03 08:06:15.000000 libvmdk-20240303/pyvmdk/pyvmdk_handle.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libfdata/libfdata.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33117 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libvmdk.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdkinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdkinfo/vmdkinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/zlib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/zlib/zlib.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5620 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_notify/vmdk_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5789 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_io_handle/vmdk_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_system_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_system_string/vmdk_test_system_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5725 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_signal/vmdk_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5813 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_descriptor/vmdk_test_extent_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_values/vmdk_test_extent_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/pyvmdk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6918 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/pyvmdk/pyvmdk.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6058 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_info_handle/vmdk_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_deflate/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_deflate/vmdk_test_deflate.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_support/vmdk_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_data/vmdk_test_grain_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6435 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_handle/vmdk_test_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_file/vmdk_test_extent_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5725 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_tools_output/vmdk_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_bit_stream/vmdk_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_compression/vmdk_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_descriptor_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5807 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_descriptor_file/vmdk_test_descriptor_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5534 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_error/vmdk_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_group/vmdk_test_grain_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23240 2024-03-03 08:33:35.000000 libvmdk-20240303/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7854 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdkmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7647 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdkmount/vmdkmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_grain_table/vmdk_test_grain_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5880 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_extent_table/vmdk_test_extent_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libvmdk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10008 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libvmdk/libvmdk.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/msvscpp/vmdk_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-03-03 08:06:41.000000 libvmdk-20240303/msvscpp/vmdk_test_huffman_tree/vmdk_test_huffman_tree.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      361 2024-03-03 08:03:12.000000 libvmdk-20240303/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30265 2024-03-03 08:33:34.000000 libvmdk-20240303/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-03 08:33:10.000000 libvmdk-20240303/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      812 2024-03-03 08:03:11.000000 libvmdk-20240303/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-03 08:33:34.000000 libvmdk-20240303/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31949 2024-03-03 08:33:34.000000 libvmdk-20240303/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:33:07.000000 libvmdk-20240303/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-03 08:03:11.000000 libvmdk-20240303/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-03-03 08:03:11.000000 libvmdk-20240303/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-03 08:33:34.000000 libvmdk-20240303/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-03 08:03:11.000000 libvmdk-20240303/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-03-03 08:03:11.000000 libvmdk-20240303/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:15.000000 libvmdk-20240303/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32355 2024-03-03 08:33:35.000000 libvmdk-20240303/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-03 08:33:16.000000 libvmdk-20240303/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      702 2024-03-03 08:03:11.000000 libvmdk-20240303/libvmdk.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-03 08:33:35.000000 libvmdk-20240303/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29543 2024-03-03 08:33:35.000000 libvmdk-20240303/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-03 08:33:14.000000 libvmdk-20240303/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1945 2023-12-03 09:15:14.000000 libvmdk-20240303/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      115 2023-12-03 09:15:28.000000 libvmdk-20240303/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1583 2024-03-03 08:03:13.000000 libvmdk-20240303/manuals/vmdkinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7490 2024-03-03 08:04:19.000000 libvmdk-20240303/manuals/libvmdk.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26356 2024-03-03 08:33:35.000000 libvmdk-20240303/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7349 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_grain_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_error.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4065 2024-03-03 08:04:12.000000 libvmdk-20240303/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20337 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_extent_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37078 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_extent_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19103 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7885 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8157 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_extent_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    68032 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_compression.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4075 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14219 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2241 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/pyvmdk_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_grain_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20439 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_extent_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14223 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/pyvmdk_test_handle.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7956 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_grain_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67992 2024-03-03 08:33:35.000000 libvmdk-20240303/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3313 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/test_vmdkinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20216 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_descriptor_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/vmdk_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53145 2024-03-03 08:03:53.000000 libvmdk-20240303/tests/vmdk_test_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4240 2024-03-03 08:03:13.000000 libvmdk-20240303/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2223 2024-03-03 08:03:13.000000 libvmdk-20240303/ossfuzz/handle_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      901 2023-12-03 09:15:30.000000 libvmdk-20240303/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-03 08:03:13.000000 libvmdk-20240303/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-03-03 08:03:13.000000 libvmdk-20240303/ossfuzz/ossfuzz_libvmdk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31747 2024-03-03 08:33:35.000000 libvmdk-20240303/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-03 08:33:28.000000 libvmdk-20240303/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30323 2024-03-03 08:33:35.000000 libvmdk-20240303/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-03 08:33:15.000000 libvmdk-20240303/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:04.000000 libvmdk-20240303/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:30.000000 libvmdk-20240303/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:30.000000 libvmdk-20240303/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:30.000000 libvmdk-20240303/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:30.000000 libvmdk-20240303/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:30.000000 libvmdk-20240303/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:30.000000 libvmdk-20240303/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:30.000000 libvmdk-20240303/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:30.000000 libvmdk-20240303/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:30.000000 libvmdk-20240303/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-03-03 08:33:47.000000 libvmdk-20240303/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:30.000000 libvmdk-20240303/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:30.000000 libvmdk-20240303/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53067 2024-03-03 08:33:35.000000 libvmdk-20240303/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-03 08:33:23.000000 libvmdk-20240303/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40459 2024-03-03 08:33:34.000000 libvmdk-20240303/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1634 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34676 2024-03-03 08:33:35.000000 libvmdk-20240303/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-03 08:33:20.000000 libvmdk-20240303/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29377 2024-03-03 08:33:35.000000 libvmdk-20240303/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-03 08:33:12.000000 libvmdk-20240303/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:03.000000 libvmdk-20240303/libvmdk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-03-03 08:33:47.000000 libvmdk-20240303/libvmdk/libvmdk.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5103 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2264 2024-03-03 08:04:12.000000 libvmdk-20240303/libvmdk/libvmdk_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9565 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52101 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48615 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12500 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8592 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   119392 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2576 2023-12-03 09:15:29.000000 libvmdk-20240303/libvmdk/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5101 2024-03-03 08:33:47.000000 libvmdk-20240303/libvmdk/libvmdk_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3377 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/vmdk_sparse_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16944 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9392 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9946 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-03-03 08:04:12.000000 libvmdk-20240303/libvmdk/libvmdk_deflate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2075 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3745 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2555 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6655 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3051 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1824 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5507 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12547 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_grain_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3184 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/cowd_sparse_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8489 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69611 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    72825 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_descriptor_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36493 2024-03-03 08:33:35.000000 libvmdk-20240303/libvmdk/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7911 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36550 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3714 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_extent_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4996 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_descriptor_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-03-03 08:03:12.000000 libvmdk-20240303/libvmdk/libvmdk_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:03:13.000000 libvmdk-20240303/libvmdk/libvmdk_libfcache.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:52:02.000000 libvmdk-20240303/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:33:08.000000 libvmdk-20240303/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28890 2024-03-03 08:33:34.000000 libvmdk-20240303/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56819 2024-03-03 08:33:31.000000 libvmdk-20240303/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7655 2024-03-03 08:03:11.000000 libvmdk-20240303/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-03-03 08:52:05.243294 libvmdk-20240303/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33350 2024-05-10 04:17:06.000000 libvmdk-20240510/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-10 04:16:51.000000 libvmdk-20240510/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3315 2024-05-10 03:58:39.000000 libvmdk-20240510/libvmdk.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-10 03:58:39.000000 libvmdk-20240510/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-10 04:17:06.000000 libvmdk-20240510/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 03:58:39.000000 libvmdk-20240510/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-10 04:17:06.000000 libvmdk-20240510/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:35.000000 libvmdk-20240510/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:29.000000 libvmdk-20240510/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-12 05:30:59.000000 libvmdk-20240510/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-10 04:17:00.000000 libvmdk-20240510/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-10 04:17:00.000000 libvmdk-20240510/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-10 04:17:00.000000 libvmdk-20240510/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-10 04:17:00.000000 libvmdk-20240510/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-10 04:17:00.000000 libvmdk-20240510/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:30.000000 libvmdk-20240510/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-10 03:58:46.000000 libvmdk-20240510/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-12 05:30:59.000000 libvmdk-20240510/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7819 2024-05-10 03:58:45.000000 libvmdk-20240510/m4/zlib.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:35.000000 libvmdk-20240510/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15626 2024-05-10 04:17:22.000000 libvmdk-20240510/include/libvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-05-10 04:02:38.000000 libvmdk-20240510/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15626 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27508 2024-05-10 04:17:06.000000 libvmdk-20240510/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:35.000000 libvmdk-20240510/include/libvmdk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3321 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3319 2024-05-10 04:17:22.000000 libvmdk-20240510/include/libvmdk/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4981 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2024-05-10 04:17:22.000000 libvmdk-20240510/include/libvmdk/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-05-10 04:17:22.000000 libvmdk-20240510/include/libvmdk/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-05-10 03:58:42.000000 libvmdk-20240510/include/libvmdk/codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-10 03:58:42.000000 libvmdk-20240510/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-10 03:58:42.000000 libvmdk-20240510/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-10 03:58:42.000000 libvmdk-20240510/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-10 03:58:42.000000 libvmdk-20240510/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-10 03:58:42.000000 libvmdk-20240510/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-10 03:58:42.000000 libvmdk-20240510/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-10 03:58:42.000000 libvmdk-20240510/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-10 04:02:38.000000 libvmdk-20240510/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-10 03:58:42.000000 libvmdk-20240510/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-05-10 04:17:22.000000 libvmdk-20240510/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16571 2024-05-10 04:17:05.000000 libvmdk-20240510/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17552 2024-05-10 04:17:23.000000 libvmdk-20240510/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-10 03:58:42.000000 libvmdk-20240510/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-10 03:58:42.000000 libvmdk-20240510/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-10 03:58:42.000000 libvmdk-20240510/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24561 2024-05-10 04:17:06.000000 libvmdk-20240510/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29759 2024-05-10 04:17:06.000000 libvmdk-20240510/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-10 04:16:43.000000 libvmdk-20240510/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:38.000000 libvmdk-20240510/vmdktools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1759 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/vmdkinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18958 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2204 2024-05-10 04:05:57.000000 libvmdk-20240510/vmdktools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20750 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20587 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15491 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/vmdkmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2702 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26617 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34230 2024-05-10 04:17:06.000000 libvmdk-20240510/vmdktools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4031 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-05-10 03:58:44.000000 libvmdk-20240510/vmdktools/vmdktools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-05-10 03:59:35.000000 libvmdk-20240510/vmdktools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-10 04:16:50.000000 libvmdk-20240510/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30268 2024-05-10 04:17:06.000000 libvmdk-20240510/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-10 04:16:50.000000 libvmdk-20240510/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-10 04:16:49.000000 libvmdk-20240510/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2411 2024-05-10 04:17:23.000000 libvmdk-20240510/libvmdk.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-05-10 04:04:04.000000 libvmdk-20240510/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33611 2024-05-10 04:17:06.000000 libvmdk-20240510/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-10 04:16:37.000000 libvmdk-20240510/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:15.000000 libvmdk-20240510/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-10 04:17:06.000000 libvmdk-20240510/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:35.000000 libvmdk-20240510/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-05-10 03:58:45.000000 libvmdk-20240510/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:35.000000 libvmdk-20240510/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2106 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/libvmdk.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-05-10 04:17:22.000000 libvmdk-20240510/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/libvmdk-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/libvmdk-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-10 03:58:39.000000 libvmdk-20240510/dpkg/libvmdk-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-05-10 04:17:23.000000 libvmdk-20240510/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-10 03:58:39.000000 libvmdk-20240510/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1843833 2024-05-10 04:17:04.000000 libvmdk-20240510/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-10 04:17:06.000000 libvmdk-20240510/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-10 04:17:06.000000 libvmdk-20240510/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:38.000000 libvmdk-20240510/pyvmdk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13199 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_libvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_disk_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_file_objects_io_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-05-10 04:04:13.000000 libvmdk-20240510/pyvmdk/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_file_objects_io_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10226 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_disk_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2590 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptors.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4736 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1631 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9785 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptors.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-10 03:58:44.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1851 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2529 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47458 2024-05-10 04:17:06.000000 libvmdk-20240510/pyvmdk/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16068 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45944 2024-05-10 03:59:35.000000 libvmdk-20240510/pyvmdk/pyvmdk_handle.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libfdata/libfdata.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33117 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/libvmdk.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdkinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdkinfo/vmdkinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/zlib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/zlib/zlib.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5620 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_notify/vmdk_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5789 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_io_handle/vmdk_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_system_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_system_string/vmdk_test_system_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5725 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_signal/vmdk_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-10 04:04:25.000000 libvmdk-20240510/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5813 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_descriptor/vmdk_test_extent_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_values/vmdk_test_extent_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/pyvmdk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6918 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/pyvmdk/pyvmdk.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6058 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_info_handle/vmdk_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_deflate/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_deflate/vmdk_test_deflate.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_support/vmdk_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_data/vmdk_test_grain_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6435 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_handle/vmdk_test_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_file/vmdk_test_extent_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5725 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_tools_output/vmdk_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_bit_stream/vmdk_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_compression/vmdk_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_descriptor_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5807 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_descriptor_file/vmdk_test_descriptor_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5534 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_error/vmdk_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_group/vmdk_test_grain_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23296 2024-05-10 04:17:06.000000 libvmdk-20240510/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7854 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdkmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7647 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdkmount/vmdkmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_grain_table/vmdk_test_grain_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5880 2024-05-10 03:59:31.000000 libvmdk-20240510/msvscpp/vmdk_test_extent_table/vmdk_test_extent_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libvmdk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10008 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libvmdk/libvmdk.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/msvscpp/vmdk_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-05-10 03:59:05.000000 libvmdk-20240510/msvscpp/vmdk_test_huffman_tree/vmdk_test_huffman_tree.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      361 2024-05-10 03:58:42.000000 libvmdk-20240510/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30592 2024-05-10 04:17:06.000000 libvmdk-20240510/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-10 04:16:42.000000 libvmdk-20240510/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      812 2024-05-10 03:58:39.000000 libvmdk-20240510/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-10 04:17:06.000000 libvmdk-20240510/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32505 2024-05-10 04:17:06.000000 libvmdk-20240510/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-10 04:16:39.000000 libvmdk-20240510/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-10 03:58:39.000000 libvmdk-20240510/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-05-10 03:58:39.000000 libvmdk-20240510/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-10 04:17:06.000000 libvmdk-20240510/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-10 03:58:39.000000 libvmdk-20240510/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-05-10 03:58:39.000000 libvmdk-20240510/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:15.000000 libvmdk-20240510/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32944 2024-05-10 04:17:06.000000 libvmdk-20240510/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-10 04:16:48.000000 libvmdk-20240510/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      702 2024-05-10 03:58:39.000000 libvmdk-20240510/libvmdk.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-10 04:17:06.000000 libvmdk-20240510/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29790 2024-05-10 04:17:06.000000 libvmdk-20240510/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-10 04:16:46.000000 libvmdk-20240510/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1945 2023-12-03 09:15:14.000000 libvmdk-20240510/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-10 04:04:57.000000 libvmdk-20240510/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1583 2024-05-10 03:58:45.000000 libvmdk-20240510/manuals/vmdkinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7490 2024-05-10 04:02:13.000000 libvmdk-20240510/manuals/libvmdk.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26520 2024-05-10 04:17:06.000000 libvmdk-20240510/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7349 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_grain_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_error.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4034 2024-05-10 04:00:31.000000 libvmdk-20240510/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20337 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_extent_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37078 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_extent_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19103 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7902 2024-05-10 04:05:45.000000 libvmdk-20240510/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8157 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_extent_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    68032 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_compression.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4405 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14219 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2241 2024-05-10 03:59:35.000000 libvmdk-20240510/tests/pyvmdk_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_grain_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20439 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_extent_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14223 2024-05-10 03:59:35.000000 libvmdk-20240510/tests/pyvmdk_test_handle.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7956 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_grain_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69358 2024-05-10 04:17:06.000000 libvmdk-20240510/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3282 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/test_vmdkinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20216 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_descriptor_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/vmdk_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53145 2024-05-10 03:59:31.000000 libvmdk-20240510/tests/vmdk_test_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4209 2024-05-10 03:58:45.000000 libvmdk-20240510/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:39.000000 libvmdk-20240510/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2223 2024-05-10 03:58:43.000000 libvmdk-20240510/ossfuzz/handle_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      897 2024-05-10 04:05:22.000000 libvmdk-20240510/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-10 03:58:43.000000 libvmdk-20240510/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-05-10 03:58:43.000000 libvmdk-20240510/ossfuzz/ossfuzz_libvmdk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31866 2024-05-10 04:17:06.000000 libvmdk-20240510/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-10 04:16:59.000000 libvmdk-20240510/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30687 2024-05-10 04:17:06.000000 libvmdk-20240510/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-10 04:16:47.000000 libvmdk-20240510/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:38.000000 libvmdk-20240510/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:30.000000 libvmdk-20240510/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:30.000000 libvmdk-20240510/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:30.000000 libvmdk-20240510/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:30.000000 libvmdk-20240510/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:30.000000 libvmdk-20240510/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:30.000000 libvmdk-20240510/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:30.000000 libvmdk-20240510/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:30.000000 libvmdk-20240510/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:30.000000 libvmdk-20240510/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-10 04:17:22.000000 libvmdk-20240510/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:30.000000 libvmdk-20240510/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:30.000000 libvmdk-20240510/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56271 2024-05-10 04:17:06.000000 libvmdk-20240510/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-10 04:16:55.000000 libvmdk-20240510/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40397 2024-05-10 04:17:06.000000 libvmdk-20240510/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:37.000000 libvmdk-20240510/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35476 2024-05-10 04:17:06.000000 libvmdk-20240510/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-10 04:16:52.000000 libvmdk-20240510/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29628 2024-05-10 04:17:06.000000 libvmdk-20240510/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-10 04:16:44.000000 libvmdk-20240510/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:38.000000 libvmdk-20240510/libvmdk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-05-10 04:17:22.000000 libvmdk-20240510/libvmdk/libvmdk.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5103 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2264 2024-05-10 03:59:43.000000 libvmdk-20240510/libvmdk/libvmdk_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9565 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52101 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48615 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12500 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8592 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   119392 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2601 2024-05-10 04:03:26.000000 libvmdk-20240510/libvmdk/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5101 2024-05-10 04:17:22.000000 libvmdk-20240510/libvmdk/libvmdk_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3377 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/vmdk_sparse_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16944 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9392 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9946 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-05-10 03:59:43.000000 libvmdk-20240510/libvmdk/libvmdk_deflate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2075 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3745 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2555 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6655 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3051 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1824 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5507 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12547 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_grain_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3184 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/cowd_sparse_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8489 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69611 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    72825 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_descriptor_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37523 2024-05-10 04:17:06.000000 libvmdk-20240510/libvmdk/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7911 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36550 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3714 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_extent_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4996 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_descriptor_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-10 03:58:43.000000 libvmdk-20240510/libvmdk/libvmdk_libfcache.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-10 04:46:36.000000 libvmdk-20240510/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-10 04:16:40.000000 libvmdk-20240510/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29095 2024-05-10 04:17:06.000000 libvmdk-20240510/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56819 2024-05-10 04:17:03.000000 libvmdk-20240510/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7655 2024-05-10 03:58:39.000000 libvmdk-20240510/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-05-10 04:46:40.318816 libvmdk-20240510/PKG-INFO
```

### Comparing `libvmdk-20240303/libfdata/libfdata_error.h` & `libvmdk-20240510/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_area.c` & `libvmdk-20240510/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_stream.h` & `libvmdk-20240510/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_cache.h` & `libvmdk-20240510/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_range_list.c` & `libvmdk-20240510/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_mapped_range.c` & `libvmdk-20240510/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_libcerror.h` & `libvmdk-20240510/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_definitions.h` & `libvmdk-20240510/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libvmdk-20240303/libfdata/libfdata_list.c` & `libvmdk-20240510/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_libcdata.h` & `libvmdk-20240510/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_list.h` & `libvmdk-20240510/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_list_element.h` & `libvmdk-20240510/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/Makefile.am` & `libvmdk-20240510/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libvmdk-20240303/libfdata/libfdata_libcnotify.h` & `libvmdk-20240510/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_extern.h` & `libvmdk-20240510/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_notify.c` & `libvmdk-20240510/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_cache.c` & `libvmdk-20240510/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_stream.c` & `libvmdk-20240510/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_unused.h` & `libvmdk-20240510/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_range.h` & `libvmdk-20240510/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_area.h` & `libvmdk-20240510/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_error.c` & `libvmdk-20240510/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_support.h` & `libvmdk-20240510/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_range.c` & `libvmdk-20240510/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_mapped_range.h` & `libvmdk-20240510/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_support.c` & `libvmdk-20240510/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_list_element.c` & `libvmdk-20240510/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_segments_array.c` & `libvmdk-20240510/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_types.h` & `libvmdk-20240510/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_notify.h` & `libvmdk-20240510/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_range_list.h` & `libvmdk-20240510/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_segments_array.h` & `libvmdk-20240510/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/Makefile.in` & `libvmdk-20240510/libfdata/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -535,16 +537,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -568,15 +570,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -788,24 +791,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -901,17 +919,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libfdata/libfdata_vector.c` & `libvmdk-20240510/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_libfcache.h` & `libvmdk-20240510/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfdata/libfdata_vector.h` & `libvmdk-20240510/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk.spec.in` & `libvmdk-20240510/libvmdk.spec.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/COPYING` & `libvmdk-20240510/COPYING`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/install-sh` & `libvmdk-20240510/install-sh`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/depcomp` & `libvmdk-20240510/depcomp`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libcfile.m4` & `libvmdk-20240510/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/tests.m4` & `libvmdk-20240510/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libcpath.m4` & `libvmdk-20240510/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/lib-prefix.m4` & `libvmdk-20240510/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/progtest.m4` & `libvmdk-20240510/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libuna.m4` & `libvmdk-20240510/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/gettext.m4` & `libvmdk-20240510/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/lib-ld.m4` & `libvmdk-20240510/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libclocale.m4` & `libvmdk-20240510/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/libcdata.m4` & `libvmdk-20240510/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/libcsplit.m4` & `libvmdk-20240510/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/common.m4` & `libvmdk-20240510/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libvmdk-20240303/m4/libcthreads.m4` & `libvmdk-20240510/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libvmdk-20240303/m4/ltversion.m4` & `libvmdk-20240510/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/ltsugar.m4` & `libvmdk-20240510/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libfdata.m4` & `libvmdk-20240510/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/host-cpu-c-abi.m4` & `libvmdk-20240510/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libfuse.m4` & `libvmdk-20240510/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libvmdk-20240303/m4/libtool.m4` & `libvmdk-20240510/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/po.m4` & `libvmdk-20240510/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libcerror.m4` & `libvmdk-20240510/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/libcnotify.m4` & `libvmdk-20240510/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/libbfio.m4` & `libvmdk-20240510/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/intlmacosx.m4` & `libvmdk-20240510/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/lt~obsolete.m4` & `libvmdk-20240510/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/lib-link.m4` & `libvmdk-20240510/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/iconv.m4` & `libvmdk-20240510/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/ltoptions.m4` & `libvmdk-20240510/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/nls.m4` & `libvmdk-20240510/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/python.m4` & `libvmdk-20240510/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libvmdk-20240303/m4/libfvalue.m4` & `libvmdk-20240510/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/types.m4` & `libvmdk-20240510/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/m4/libfcache.m4` & `libvmdk-20240510/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libvmdk-20240303/m4/pthread.m4` & `libvmdk-20240510/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libvmdk-20240303/m4/zlib.m4` & `libvmdk-20240510/m4/zlib.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for zlib required headers and functions
 dnl
-dnl Version: 20201230
+dnl Version: 20240314
 
 dnl Function to detect if zlib is available
 AC_DEFUN([AX_ZLIB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno],
     [ac_cv_zlib=no],
     [ac_cv_zlib=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-zlib which returns "yes" and --with-zlib= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect],
+      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_zlib"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_zlib],
           [1])
@@ -58,14 +60,21 @@
             [Missing function: zlibVersion in library: zlib.],
             [1])
           ])
 
         ac_cv_zlib_LIBADD="-lz";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported zlib in directory: $ac_cv_with_zlib],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_zlib" = xzlib],
     [AC_DEFINE(
       [HAVE_ZLIB],
       [1],
```

### Comparing `libvmdk-20240303/include/libvmdk.h` & `libvmdk-20240510/include/libvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk.h.in` & `libvmdk-20240510/include/libvmdk.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/Makefile.in` & `libvmdk-20240510/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -437,14 +437,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -517,15 +519,20 @@
 
 EXTRA_DIST = \
 	libvmdk.h.in \
 	libvmdk/definitions.h.in \
 	libvmdk/features.h.in \
 	libvmdk/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvmdk.h \
+	libvmdk/definitions.h \
+	libvmdk/features.h \
+	libvmdk/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -722,23 +729,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -820,17 +829,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvmdk.h
-	-rm -f libvmdk/definitions.h
-	-rm -f libvmdk/features.h
-	-rm -f libvmdk/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/include/libvmdk/definitions.h.in` & `libvmdk-20240510/include/libvmdk/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/definitions.h` & `libvmdk-20240510/include/libvmdk/definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVMDK_DEFINITIONS_H )
 #define _LIBVMDK_DEFINITIONS_H
 
 #include <libvmdk/types.h>
 
-#define LIBVMDK_VERSION				20240303
+#define LIBVMDK_VERSION				20240510
 
 /* The version string
  */
-#define LIBVMDK_VERSION_STRING			"20240303"
+#define LIBVMDK_VERSION_STRING			"20240510"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVMDK_ACCESS_FLAGS
```

### Comparing `libvmdk-20240303/include/libvmdk/types.h.in` & `libvmdk-20240510/include/libvmdk/types.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/types.h` & `libvmdk-20240510/include/libvmdk/types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/features.h.in` & `libvmdk-20240510/include/libvmdk/features.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/error.h` & `libvmdk-20240510/include/libvmdk/error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/extern.h` & `libvmdk-20240510/include/libvmdk/extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/features.h` & `libvmdk-20240510/include/libvmdk/features.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/include/libvmdk/codepage.h` & `libvmdk-20240510/include/libvmdk/codepage.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/config_borlandc.h` & `libvmdk-20240510/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/file_stream.h` & `libvmdk-20240510/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/memory.h` & `libvmdk-20240510/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/byte_stream.h` & `libvmdk-20240510/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/common.h` & `libvmdk-20240510/common/common.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/config_winapi.h` & `libvmdk-20240510/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/system_string.h` & `libvmdk-20240510/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/types.h.in` & `libvmdk-20240510/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/types.h` & `libvmdk-20240510/common/types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/config.h.in` & `libvmdk-20240510/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,17 @@
 
 /* Define to 1 if you have the <libfdata.h> header file. */
 #undef HAVE_LIBFDATA_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 #undef HAVE_LIBFVALUE
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 #undef HAVE_LIBFVALUE_H
 
 /* Define to 1 if you have the <libintl.h> header file. */
```

### Comparing `libvmdk-20240303/common/config.h` & `libvmdk-20240510/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,18 @@
 /* Define to 1 if you have the `fdata' library (-lfdata). */
 /* #undef HAVE_LIBFDATA */
 
 /* Define to 1 if you have the <libfdata.h> header file. */
 /* #undef HAVE_LIBFDATA_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 /* #undef HAVE_LIBFVALUE */
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 /* #undef HAVE_LIBFVALUE_H */
 
@@ -544,24 +547,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvmdk"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvmdk 20240303"
+#define PACKAGE_STRING "libvmdk 20240510"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvmdk"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240303"
+#define PACKAGE_VERSION "20240510"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -582,15 +585,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240303"
+#define VERSION "20240510"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvmdk-20240303/common/wide_string.h` & `libvmdk-20240510/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/narrow_string.h` & `libvmdk-20240510/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/config_msc.h` & `libvmdk-20240510/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/common/Makefile.in` & `libvmdk-20240510/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -470,15 +472,17 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -486,15 +490,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -662,23 +669,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -758,15 +767,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/libclocale/libclocale_wide_string.c` & `libvmdk-20240510/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_support.h` & `libvmdk-20240510/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/Makefile.am` & `libvmdk-20240510/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libvmdk-20240303/libclocale/libclocale_definitions.h` & `libvmdk-20240510/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libvmdk-20240303/libclocale/libclocale_unused.h` & `libvmdk-20240510/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_libcerror.h` & `libvmdk-20240510/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_locale.h` & `libvmdk-20240510/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_support.c` & `libvmdk-20240510/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_codepage.c` & `libvmdk-20240510/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_locale.c` & `libvmdk-20240510/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/Makefile.in` & `libvmdk-20240510/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -516,30 +518,31 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -742,24 +745,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -846,17 +855,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libclocale/libclocale_extern.h` & `libvmdk-20240510/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_wide_string.h` & `libvmdk-20240510/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libclocale/libclocale_codepage.h` & `libvmdk-20240510/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_dokan.c` & `libvmdk-20240510/vmdktools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libfvalue.h` & `libvmdk-20240510/vmdktools/vmdktools_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_file_system.h` & `libvmdk-20240510/vmdktools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdkinfo.c` & `libvmdk-20240510/vmdktools/vmdkinfo.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_fuse.c` & `libvmdk-20240510/vmdktools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/info_handle.h` & `libvmdk-20240510/vmdktools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_getopt.h` & `libvmdk-20240510/vmdktools/vmdktools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_dokan.h` & `libvmdk-20240510/vmdktools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_file_system.c` & `libvmdk-20240510/vmdktools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libvmdk.h` & `libvmdk-20240510/vmdktools/vmdktools_libvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/byte_size_string.c` & `libvmdk-20240510/vmdktools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/Makefile.am` & `libvmdk-20240510/vmdktools/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -75,19 +75,17 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvmdk/libvmdk.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vmdkinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vmdkinfo_SOURCES)
 	@echo "Running splint on vmdkmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vmdkmount_SOURCES)
```

### Comparing `libvmdk-20240303/vmdktools/vmdktools_i18n.h` & `libvmdk-20240510/vmdktools/vmdktools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_file_entry.c` & `libvmdk-20240510/vmdktools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/info_handle.c` & `libvmdk-20240510/vmdktools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libclocale.h` & `libvmdk-20240510/vmdktools/vmdktools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_file_entry.h` & `libvmdk-20240510/vmdktools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdkmount.c` & `libvmdk-20240510/vmdktools/vmdkmount.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_signal.c` & `libvmdk-20240510/vmdktools/vmdktools_signal.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_handle.h` & `libvmdk-20240510/vmdktools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libuna.h` & `libvmdk-20240510/vmdktools/vmdktools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_getopt.c` & `libvmdk-20240510/vmdktools/vmdktools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libcdata.h` & `libvmdk-20240510/vmdktools/vmdktools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libcpath.h` & `libvmdk-20240510/vmdktools/vmdktools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_signal.h` & `libvmdk-20240510/vmdktools/vmdktools_signal.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_output.h` & `libvmdk-20240510/vmdktools/vmdktools_output.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_handle.c` & `libvmdk-20240510/vmdktools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_unused.h` & `libvmdk-20240510/vmdktools/vmdktools_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/Makefile.in` & `libvmdk-20240510/vmdktools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -455,14 +455,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -519,16 +521,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -594,15 +596,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvmdk/libvmdk.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -859,23 +862,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/vmdkinfo.Po
+	-rm -f ./$(DEPDIR)/vmdkmount.Po
+	-rm -f ./$(DEPDIR)/vmdktools_getopt.Po
+	-rm -f ./$(DEPDIR)/vmdktools_output.Po
+	-rm -f ./$(DEPDIR)/vmdktools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -970,17 +987,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vmdkinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vmdkinfo_SOURCES)
 	@echo "Running splint on vmdkmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vmdkmount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libcnotify.h` & `libvmdk-20240510/vmdktools/vmdktools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/byte_size_string.h` & `libvmdk-20240510/vmdktools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_output.c` & `libvmdk-20240510/vmdktools/vmdktools_output.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libbfio.h` & `libvmdk-20240510/vmdktools/vmdktools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/vmdktools_libcerror.h` & `libvmdk-20240510/vmdktools/vmdktools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/vmdktools/mount_fuse.h` & `libvmdk-20240510/vmdktools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_libcdata.h` & `libvmdk-20240510/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_types.h` & `libvmdk-20240510/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_cache_value.c` & `libvmdk-20240510/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_unused.h` & `libvmdk-20240510/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/Makefile.am` & `libvmdk-20240510/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libvmdk-20240303/libfcache/libfcache_support.h` & `libvmdk-20240510/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_error.h` & `libvmdk-20240510/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_support.c` & `libvmdk-20240510/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_cache.h` & `libvmdk-20240510/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_error.c` & `libvmdk-20240510/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_libcerror.h` & `libvmdk-20240510/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_date_time.c` & `libvmdk-20240510/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_extern.h` & `libvmdk-20240510/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_cache_value.h` & `libvmdk-20240510/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/Makefile.in` & `libvmdk-20240510/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -518,16 +520,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -539,15 +541,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -751,24 +754,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -856,17 +866,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libfcache/libfcache_date_time.h` & `libvmdk-20240510/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfcache/libfcache_definitions.h` & `libvmdk-20240510/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libvmdk-20240303/libfcache/libfcache_cache.c` & `libvmdk-20240510/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk.spec` & `libvmdk-20240510/libvmdk.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvmdk
-Version: 20240303
+Version: 20240510
 Release: 1
 Summary: Library to access the VMware Virtual Disk (VMDK) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvmdk
 Requires:              zlib
@@ -36,16 +36,16 @@
 
 %description -n libvmdk-python3
 Python 3 bindings for libvmdk
 
 %package -n libvmdk-tools
 Summary: Several tools for reading VMware Virtual Disk (VMDK) files
 Group: Applications/System
-Requires: libvmdk = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libvmdk = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libvmdk-tools
 Several tools for reading VMware Virtual Disk (VMDK) files
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libvmdk-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sun Mar  3 2024 Joachim Metz <joachim.metz@gmail.com> 20240303-1
+* Fri May 10 2024 Joachim Metz <joachim.metz@gmail.com> 20240510-1
 - Auto-generated
```

### Comparing `libvmdk-20240303/Makefile.am` & `libvmdk-20240510/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -58,16 +58,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvmdk.pc \
+	libvmdk.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libvmdk.pc
 
 libtool:
@@ -90,19 +97,7 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvmdk && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvmdk.pc
-	-rm -f libvmdk.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_range.h` & `libvmdk-20240510/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_range_io_handle.c` & `libvmdk-20240510/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_support.c` & `libvmdk-20240510/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libcpath.h` & `libvmdk-20240510/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_error.h` & `libvmdk-20240510/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libclocale.h` & `libvmdk-20240510/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_error.c` & `libvmdk-20240510/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libuna.h` & `libvmdk-20240510/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_io_handle.h` & `libvmdk-20240510/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_pool.h` & `libvmdk-20240510/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_range.c` & `libvmdk-20240510/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_types.h` & `libvmdk-20240510/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_unused.h` & `libvmdk-20240510/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libcdata.h` & `libvmdk-20240510/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file.h` & `libvmdk-20240510/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/Makefile.am` & `libvmdk-20240510/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libcfile.h` & `libvmdk-20240510/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_definitions.h` & `libvmdk-20240510/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libvmdk-20240303/libbfio/libbfio_codepage.h` & `libvmdk-20240510/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_io_handle.c` & `libvmdk-20240510/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_support.h` & `libvmdk-20240510/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_memory_range.h` & `libvmdk-20240510/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_pool.c` & `libvmdk-20240510/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file_range_io_handle.h` & `libvmdk-20240510/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libcthreads.h` & `libvmdk-20240510/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_system_string.h` & `libvmdk-20240510/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_memory_range_io_handle.c` & `libvmdk-20240510/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_handle.c` & `libvmdk-20240510/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_file.c` & `libvmdk-20240510/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_handle.h` & `libvmdk-20240510/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_memory_range.c` & `libvmdk-20240510/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_pool.c` & `libvmdk-20240510/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_libcerror.h` & `libvmdk-20240510/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/Makefile.in` & `libvmdk-20240510/libbfio/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -576,15 +578,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -795,24 +798,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -881,14 +898,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -899,23 +918,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/libbfio/libbfio_system_string.c` & `libvmdk-20240510/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_memory_range_io_handle.h` & `libvmdk-20240510/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_extern.h` & `libvmdk-20240510/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/libbfio/libbfio_pool.h` & `libvmdk-20240510/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvmdk-20240303/config.guess` & `libvmdk-20240510/config.guess`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/dpkg/copyright` & `libvmdk-20240510/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/dpkg/control` & `libvmdk-20240510/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/dpkg/rules` & `libvmdk-20240510/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/COPYING.LESSER` & `libvmdk-20240510/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/configure` & `libvmdk-20240510/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvmdk 20240303.
+# Generated by GNU Autoconf 2.71 for libvmdk 20240510.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libvmdk'
 PACKAGE_TARNAME='libvmdk'
-PACKAGE_VERSION='20240303'
-PACKAGE_STRING='libvmdk 20240303'
+PACKAGE_VERSION='20240510'
+PACKAGE_STRING='libvmdk 20240510'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvmdk.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1100,14 +1102,16 @@
 libfcache_LIBS
 libfdata_CFLAGS
 libfdata_LIBS
 libfvalue_CFLAGS
 libfvalue_LIBS
 zlib_CFLAGS
 zlib_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1650,15 +1654,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvmdk 20240303 to adapt to many kinds of systems.
+\`configure' configures libvmdk 20240510 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1721,15 +1725,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvmdk 20240303:";;
+     short | recursive ) echo "Configuration of libvmdk 20240510:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1898,14 +1902,17 @@
               linker flags for libfdata, overriding pkg-config
   libfvalue_CFLAGS
               C compiler flags for libfvalue, overriding pkg-config
   libfvalue_LIBS
               linker flags for libfvalue, overriding pkg-config
   zlib_CFLAGS C compiler flags for zlib, overriding pkg-config
   zlib_LIBS   linker flags for zlib, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1968,15 +1975,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvmdk configure 20240303
+libvmdk configure 20240510
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2689,15 +2696,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvmdk $as_me 20240303, which was
+It was created by libvmdk $as_me 20240510, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4178,15 +4185,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvmdk'
- VERSION='20240303'
+ VERSION='20240510'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23773,15 +23780,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24272,15 +24279,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24422,15 +24430,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24524,15 +24532,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26164,15 +26172,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26226,47 +26234,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26300,15 +26313,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26342,15 +26355,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26385,15 +26398,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26427,15 +26440,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26469,15 +26482,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26511,15 +26524,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26553,15 +26566,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26596,15 +26609,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26638,15 +26651,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26680,15 +26693,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26722,15 +26735,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26764,15 +26777,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26807,15 +26820,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26849,15 +26862,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26891,15 +26904,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26933,15 +26946,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26975,15 +26988,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27018,67 +27031,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27166,15 +27188,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30945,15 +30967,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30978,15 +31001,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31056,15 +31079,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31611,15 +31634,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31775,15 +31799,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31853,15 +31877,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32311,15 +32335,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32374,15 +32399,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32452,15 +32477,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33175,15 +33200,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33208,15 +33234,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33286,15 +33312,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40496,15 +40522,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40529,15 +40556,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40607,15 +40634,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41796,15 +41823,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42118,15 +42146,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42196,15 +42224,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43001,15 +43029,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43199,15 +43228,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43277,15 +43306,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45395,15 +45424,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45428,15 +45458,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45506,15 +45536,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46426,15 +46456,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46527,15 +46558,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46605,15 +46636,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49893,15 +49924,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49926,15 +49958,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50004,15 +50036,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54318,15 +54350,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54351,15 +54384,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -54429,15 +54462,15 @@
 printf "%s\n" "$ac_cv_with_zlib" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno
 then :
   ac_cv_zlib=no
 else $as_nop
   ac_cv_zlib=check
-        if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect
+                if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
 then :
   if test -d "$ac_cv_with_zlib"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54604,14 +54637,23 @@
 
         ac_cv_zlib_LIBADD="-lz";
 
 fi
 
 fi
 
+    if test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported zlib in directory: $ac_cv_with_zlib
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_zlib" = xzlib
 then :
 
 printf "%s\n" "#define HAVE_ZLIB 1" >>confdefs.h
 
@@ -54983,16 +55025,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -55150,33 +55196,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -55244,51 +55364,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -55451,45 +55630,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -55657,29 +55829,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -55710,14 +55902,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -55725,14 +55923,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -56646,15 +56852,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvmdk $as_me 20240303, which was
+This file was extended by libvmdk $as_me 20240510, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -56714,15 +56920,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvmdk config.status 20240303
+libvmdk config.status 20240510
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvmdk-20240303/compile` & `libvmdk-20240510/compile`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/missing` & `libvmdk-20240510/missing`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_file_object_io_handle.h` & `libvmdk-20240510/pyvmdk/pyvmdk_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptor.c` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_libvmdk.h` & `libvmdk-20240510/pyvmdk/pyvmdk_libvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_libcerror.h` & `libvmdk-20240510/pyvmdk/pyvmdk_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_disk_types.h` & `libvmdk-20240510/pyvmdk/pyvmdk_disk_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_unused.h` & `libvmdk-20240510/pyvmdk/pyvmdk_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_integer.c` & `libvmdk-20240510/pyvmdk/pyvmdk_integer.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_libbfio.h` & `libvmdk-20240510/pyvmdk/pyvmdk_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_file_objects_io_pool.h` & `libvmdk-20240510/pyvmdk/pyvmdk_file_objects_io_pool.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/Makefile.am` & `libvmdk-20240510/pyvmdk/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -44,13 +44,11 @@
 	@LIBBFIO_LIBADD@
 
 pyvmdk_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyvmdk_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_file_object_io_handle.c` & `libvmdk-20240510/pyvmdk/pyvmdk_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_error.h` & `libvmdk-20240510/pyvmdk/pyvmdk_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_python.h` & `libvmdk-20240510/pyvmdk/pyvmdk_python.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_file_objects_io_pool.c` & `libvmdk-20240510/pyvmdk/pyvmdk_file_objects_io_pool.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_disk_types.c` & `libvmdk-20240510/pyvmdk/pyvmdk_disk_types.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptors.h` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptors.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_handle.h` & `libvmdk-20240510/pyvmdk/pyvmdk_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_libclocale.h` & `libvmdk-20240510/pyvmdk/pyvmdk_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_types.h` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_error.c` & `libvmdk-20240510/pyvmdk/pyvmdk_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptors.c` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptors.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_integer.h` & `libvmdk-20240510/pyvmdk/pyvmdk_integer.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_types.c` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_types.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk.h` & `libvmdk-20240510/pyvmdk/pyvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_extent_descriptor.h` & `libvmdk-20240510/pyvmdk/pyvmdk_extent_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/Makefile.in` & `libvmdk-20240510/pyvmdk/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -498,14 +498,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -562,16 +564,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -606,15 +608,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyvmdk_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyvmdk_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -920,24 +923,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_disk_types.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_error.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_extent_descriptor.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_extent_descriptors.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_extent_types.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_file_objects_io_pool.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvmdk_la-pyvmdk_integer.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1031,13 +1046,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk.c` & `libvmdk-20240510/pyvmdk/pyvmdk.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/pyvmdk/pyvmdk_handle.c` & `libvmdk-20240510/pyvmdk/pyvmdk_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libfdata/libfdata.vcproj` & `libvmdk-20240510/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libvmdk.sln` & `libvmdk-20240510/msvscpp/libvmdk.sln`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdkinfo/vmdkinfo.vcproj` & `libvmdk-20240510/msvscpp/vmdkinfo/vmdkinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/zlib/zlib.vcproj` & `libvmdk-20240510/msvscpp/zlib/zlib.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_notify/vmdk_test_notify.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_notify/vmdk_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_io_handle/vmdk_test_io_handle.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_io_handle/vmdk_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_system_string/vmdk_test_system_string.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_system_string/vmdk_test_system_string.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_tools_signal/vmdk_test_tools_signal.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_tools_signal/vmdk_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libclocale/libclocale.vcproj` & `libvmdk-20240510/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libfcache/libfcache.vcproj` & `libvmdk-20240510/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/Makefile.am` & `libvmdk-20240510/msvscpp/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -39,13 +39,11 @@
 	vmdkmount/vmdkmount.vcproj \
 	zlib/zlib.vcproj \
 	libvmdk.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvmdk-20240303/msvscpp/libbfio/libbfio.vcproj` & `libvmdk-20240510/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_extent_descriptor/vmdk_test_extent_descriptor.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_extent_descriptor/vmdk_test_extent_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_extent_values/vmdk_test_extent_values.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_extent_values/vmdk_test_extent_values.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/pyvmdk/pyvmdk.vcproj` & `libvmdk-20240510/msvscpp/pyvmdk/pyvmdk.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_tools_info_handle/vmdk_test_tools_info_handle.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_tools_info_handle/vmdk_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcfile/libcfile.vcproj` & `libvmdk-20240510/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_deflate/vmdk_test_deflate.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_deflate/vmdk_test_deflate.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcdata/libcdata.vcproj` & `libvmdk-20240510/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_support/vmdk_test_support.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_support/vmdk_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_grain_data/vmdk_test_grain_data.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_grain_data/vmdk_test_grain_data.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_handle/vmdk_test_handle.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_handle/vmdk_test_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_extent_file/vmdk_test_extent_file.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_extent_file/vmdk_test_extent_file.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_tools_output/vmdk_test_tools_output.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_tools_output/vmdk_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_bit_stream/vmdk_test_bit_stream.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_bit_stream/vmdk_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcthreads/libcthreads.vcproj` & `libvmdk-20240510/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_compression/vmdk_test_compression.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_compression/vmdk_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_descriptor_file/vmdk_test_descriptor_file.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_descriptor_file/vmdk_test_descriptor_file.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcpath/libcpath.vcproj` & `libvmdk-20240510/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_error/vmdk_test_error.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_error/vmdk_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcsplit/libcsplit.vcproj` & `libvmdk-20240510/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_grain_group/vmdk_test_grain_group.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_grain_group/vmdk_test_grain_group.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libuna/libuna.vcproj` & `libvmdk-20240510/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/Makefile.in` & `libvmdk-20240510/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -497,15 +499,16 @@
 	vmdkmount/vmdkmount.vcproj \
 	zlib/zlib.vcproj \
 	libvmdk.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -609,23 +612,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -704,13 +709,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/msvscpp/libfvalue/libfvalue.vcproj` & `libvmdk-20240510/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdkmount/vmdkmount.vcproj` & `libvmdk-20240510/msvscpp/vmdkmount/vmdkmount.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_grain_table/vmdk_test_grain_table.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_grain_table/vmdk_test_grain_table.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_extent_table/vmdk_test_extent_table.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_extent_table/vmdk_test_extent_table.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcnotify/libcnotify.vcproj` & `libvmdk-20240510/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libvmdk/libvmdk.vcproj` & `libvmdk-20240510/msvscpp/libvmdk/libvmdk.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/libcerror/libcerror.vcproj` & `libvmdk-20240510/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/msvscpp/vmdk_test_huffman_tree/vmdk_test_huffman_tree.vcproj` & `libvmdk-20240510/msvscpp/vmdk_test_huffman_tree/vmdk_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_extern.h` & `libvmdk-20240510/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_support.h` & `libvmdk-20240510/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_unused.h` & `libvmdk-20240510/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_notify.h` & `libvmdk-20240510/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_support.c` & `libvmdk-20240510/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_types.h` & `libvmdk-20240510/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/Makefile.am` & `libvmdk-20240510/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcfile/libcfile_notify.c` & `libvmdk-20240510/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_system_string.h` & `libvmdk-20240510/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_file.h` & `libvmdk-20240510/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_libcnotify.h` & `libvmdk-20240510/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_system_string.c` & `libvmdk-20240510/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_error.h` & `libvmdk-20240510/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_libcerror.h` & `libvmdk-20240510/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_file.c` & `libvmdk-20240510/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_libclocale.h` & `libvmdk-20240510/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_winapi.h` & `libvmdk-20240510/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/Makefile.in` & `libvmdk-20240510/libcfile/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -518,16 +520,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -542,15 +544,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -755,24 +758,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -861,17 +872,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcfile/libcfile_error.c` & `libvmdk-20240510/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_libuna.h` & `libvmdk-20240510/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_winapi.c` & `libvmdk-20240510/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcfile/libcfile_definitions.h` & `libvmdk-20240510/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libvmdk-20240303/README` & `libvmdk-20240510/README`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/INSTALL` & `libvmdk-20240510/INSTALL`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_list_element.h` & `libvmdk-20240510/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_array.h` & `libvmdk-20240510/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_definitions.h` & `libvmdk-20240510/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvmdk-20240303/libcdata/libcdata_libcerror.h` & `libvmdk-20240510/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_unused.h` & `libvmdk-20240510/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_btree.h` & `libvmdk-20240510/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_btree.c` & `libvmdk-20240510/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_support.c` & `libvmdk-20240510/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_list.c` & `libvmdk-20240510/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_extern.h` & `libvmdk-20240510/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_list.h` & `libvmdk-20240510/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_btree_values_list.h` & `libvmdk-20240510/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/Makefile.am` & `libvmdk-20240510/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcdata/libcdata_btree_node.h` & `libvmdk-20240510/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_range_list_value.h` & `libvmdk-20240510/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_range_list.h` & `libvmdk-20240510/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_range_list.c` & `libvmdk-20240510/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_array.c` & `libvmdk-20240510/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_list_element.c` & `libvmdk-20240510/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_libcthreads.h` & `libvmdk-20240510/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_tree_node.h` & `libvmdk-20240510/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_error.h` & `libvmdk-20240510/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_types.h` & `libvmdk-20240510/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_btree_node.c` & `libvmdk-20240510/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_tree_node.c` & `libvmdk-20240510/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_support.h` & `libvmdk-20240510/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/Makefile.in` & `libvmdk-20240510/libcdata/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -532,16 +534,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -558,15 +560,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -776,24 +779,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -887,17 +903,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcdata/libcdata_range_list_value.c` & `libvmdk-20240510/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_btree_values_list.c` & `libvmdk-20240510/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcdata/libcdata_error.c` & `libvmdk-20240510/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/config.sub` & `libvmdk-20240510/config.sub`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/setup.py` & `libvmdk-20240510/setup.py`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/acinclude.m4` & `libvmdk-20240510/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/config.rpath` & `libvmdk-20240510/config.rpath`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread.h` & `libvmdk-20240510/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_read_write_lock.h` & `libvmdk-20240510/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread.c` & `libvmdk-20240510/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread_pool.h` & `libvmdk-20240510/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_support.h` & `libvmdk-20240510/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_lock.h` & `libvmdk-20240510/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_unused.h` & `libvmdk-20240510/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_lock.c` & `libvmdk-20240510/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_condition.h` & `libvmdk-20240510/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_repeating_thread.h` & `libvmdk-20240510/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/Makefile.am` & `libvmdk-20240510/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcthreads/libcthreads_support.c` & `libvmdk-20240510/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_mutex.c` & `libvmdk-20240510/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_queue.c` & `libvmdk-20240510/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_mutex.h` & `libvmdk-20240510/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_types.h` & `libvmdk-20240510/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread_attributes.h` & `libvmdk-20240510/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_condition.c` & `libvmdk-20240510/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_error.c` & `libvmdk-20240510/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_read_write_lock.c` & `libvmdk-20240510/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_libcerror.h` & `libvmdk-20240510/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_definitions.h` & `libvmdk-20240510/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread_pool.c` & `libvmdk-20240510/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_error.h` & `libvmdk-20240510/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_thread_attributes.c` & `libvmdk-20240510/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_extern.h` & `libvmdk-20240510/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/libcthreads_repeating_thread.c` & `libvmdk-20240510/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcthreads/Makefile.in` & `libvmdk-20240510/libcthreads/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -560,15 +562,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -778,24 +781,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -889,17 +905,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcthreads/libcthreads_queue.h` & `libvmdk-20240510/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk.pc.in` & `libvmdk-20240510/libvmdk.pc.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/test-driver` & `libvmdk-20240510/test-driver`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_support.c` & `libvmdk-20240510/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_libcerror.h` & `libvmdk-20240510/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_definitions.h` & `libvmdk-20240510/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libvmdk-20240303/libcpath/Makefile.am` & `libvmdk-20240510/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcpath/libcpath_error.c` & `libvmdk-20240510/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_extern.h` & `libvmdk-20240510/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_system_string.h` & `libvmdk-20240510/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_support.h` & `libvmdk-20240510/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_libcsplit.h` & `libvmdk-20240510/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_system_string.c` & `libvmdk-20240510/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_libclocale.h` & `libvmdk-20240510/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_error.h` & `libvmdk-20240510/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/Makefile.in` & `libvmdk-20240510/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -448,14 +448,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,16 +514,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -533,15 +535,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -744,24 +747,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -848,17 +857,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcpath/libcpath_libuna.h` & `libvmdk-20240510/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_unused.h` & `libvmdk-20240510/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_path.c` & `libvmdk-20240510/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcpath/libcpath_path.h` & `libvmdk-20240510/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/ChangeLog` & `libvmdk-20240510/ChangeLog`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/manuals/vmdkinfo.1` & `libvmdk-20240510/manuals/vmdkinfo.1`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/manuals/libvmdk.3` & `libvmdk-20240510/manuals/libvmdk.3`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/manuals/Makefile.in` & `libvmdk-20240510/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -492,14 +494,18 @@
 	vmdkinfo.1 \
 	libvmdk.3
 
 man_MANS = \
 	vmdkinfo.1 \
 	libvmdk.3
 
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in
+
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
 	  case '$(am__configure_deps)' in \
 	    *$$dep*) \
@@ -690,22 +696,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -787,13 +796,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/tests/vmdk_test_memory.h` & `libvmdk-20240510/tests/vmdk_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_notify.c` & `libvmdk-20240510/tests/vmdk_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_grain_table.c` & `libvmdk-20240510/tests/vmdk_test_grain_table.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_libuna.h` & `libvmdk-20240510/tests/vmdk_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_error.c` & `libvmdk-20240510/tests/vmdk_test_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/test_tools.sh` & `libvmdk-20240510/tests/test_tools.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvmdk-20240303/tests/vmdk_test_bit_stream.c` & `libvmdk-20240510/tests/vmdk_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_libvmdk.h` & `libvmdk-20240510/tests/vmdk_test_libvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_extent_descriptor.c` & `libvmdk-20240510/tests/vmdk_test_extent_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_extent_table.c` & `libvmdk-20240510/tests/vmdk_test_extent_table.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_memory.c` & `libvmdk-20240510/tests/vmdk_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_system_string.c` & `libvmdk-20240510/tests/vmdk_test_system_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/Makefile.am` & `libvmdk-20240510/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -342,13 +342,12 @@
 	vmdk_test_tools_signal.c \
 	vmdk_test_unused.h
 
 vmdk_test_tools_signal_LDADD = \
 	../libvmdk/libvmdk.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libvmdk-20240303/tests/vmdk_test_libcpath.h` & `libvmdk-20240510/tests/vmdk_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_tools_signal.c` & `libvmdk-20240510/tests/vmdk_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_functions.h` & `libvmdk-20240510/tests/vmdk_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_libclocale.h` & `libvmdk-20240510/tests/vmdk_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_extent_file.c` & `libvmdk-20240510/tests/vmdk_test_extent_file.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_compression.c` & `libvmdk-20240510/tests/vmdk_test_compression.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/test_python_module.sh` & `libvmdk-20240510/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="handle";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libvmdk";
+PYTHON_MODULE="pyvmdk";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvmdk_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvmdk_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyvmdk");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libvmdk-20240303/tests/vmdk_test_deflate.c` & `libvmdk-20240510/tests/vmdk_test_deflate.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_getopt.h` & `libvmdk-20240510/tests/vmdk_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_getopt.c` & `libvmdk-20240510/tests/vmdk_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_support.c` & `libvmdk-20240510/tests/vmdk_test_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_tools_output.c` & `libvmdk-20240510/tests/vmdk_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/pyvmdk_test_support.py` & `libvmdk-20240510/tests/pyvmdk_test_support.py`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/test_runner.sh` & `libvmdk-20240510/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_huffman_tree.c` & `libvmdk-20240510/tests/vmdk_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_grain_group.c` & `libvmdk-20240510/tests/vmdk_test_grain_group.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_libcnotify.h` & `libvmdk-20240510/tests/vmdk_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_extent_values.c` & `libvmdk-20240510/tests/vmdk_test_extent_values.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/pyvmdk_test_handle.py` & `libvmdk-20240510/tests/pyvmdk_test_handle.py`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_unused.h` & `libvmdk-20240510/tests/vmdk_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_functions.c` & `libvmdk-20240510/tests/vmdk_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_io_handle.c` & `libvmdk-20240510/tests/vmdk_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_grain_data.c` & `libvmdk-20240510/tests/vmdk_test_grain_data.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/Makefile.in` & `libvmdk-20240510/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -806,14 +806,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -871,16 +873,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1191,16 +1193,18 @@
 	vmdk_test_tools_signal.c \
 	vmdk_test_unused.h
 
 vmdk_test_tools_signal_LDADD = \
 	../libvmdk/libvmdk.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1714,24 +1718,54 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../vmdktools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../vmdktools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../vmdktools/$(DEPDIR)/byte_size_string.Po
+	-rm -f ../vmdktools/$(DEPDIR)/info_handle.Po
+	-rm -f ../vmdktools/$(DEPDIR)/vmdktools_output.Po
+	-rm -f ../vmdktools/$(DEPDIR)/vmdktools_signal.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_compression.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_deflate.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_descriptor_file.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_error.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_extent_descriptor.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_extent_file.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_extent_table.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_extent_values.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_functions.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_getopt.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_grain_data.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_grain_group.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_grain_table.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_handle.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_memory.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_notify.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_support.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_system_string.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/vmdk_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1842,13 +1876,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/tests/vmdk_test_libbfio.h` & `libvmdk-20240510/tests/vmdk_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/test_vmdkinfo.sh` & `libvmdk-20240510/tests/test_vmdkinfo.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("vmdkinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvmdk-20240303/tests/vmdk_test_tools_info_handle.c` & `libvmdk-20240510/tests/vmdk_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_libcerror.h` & `libvmdk-20240510/tests/vmdk_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_descriptor_file.c` & `libvmdk-20240510/tests/vmdk_test_descriptor_file.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_macros.h` & `libvmdk-20240510/tests/vmdk_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/vmdk_test_handle.c` & `libvmdk-20240510/tests/vmdk_test_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/tests/test_library.sh` & `libvmdk-20240510/tests/test_library.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="bit_stream compression deflate descriptor_file error extent_descriptor extent_file extent_table extent_values grain_data grain_group grain_table huffman_tree io_handle notify system_string";
 LIBRARY_TESTS_WITH_INPUT="handle support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvmdk-20240303/ossfuzz/handle_fuzzer.cc` & `libvmdk-20240510/ossfuzz/handle_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/ossfuzz/Makefile.am` & `libvmdk-20240510/ossfuzz/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libvmdk/libvmdk.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
```

### Comparing `libvmdk-20240303/ossfuzz/ossfuzz_libbfio.h` & `libvmdk-20240510/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/ossfuzz/ossfuzz_libvmdk.h` & `libvmdk-20240510/ossfuzz/ossfuzz_libvmdk.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/ossfuzz/Makefile.in` & `libvmdk-20240510/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -525,16 +527,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -554,15 +556,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libvmdk/libvmdk.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,23 +807,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/handle_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -904,17 +910,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/ltmain.sh` & `libvmdk-20240510/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_narrow_string.c` & `libvmdk-20240510/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_definitions.h` & `libvmdk-20240510/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libvmdk-20240303/libcsplit/libcsplit_types.h` & `libvmdk-20240510/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_wide_split_string.c` & `libvmdk-20240510/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_support.h` & `libvmdk-20240510/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/Makefile.am` & `libvmdk-20240510/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcsplit/libcsplit_libcerror.h` & `libvmdk-20240510/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_wide_string.c` & `libvmdk-20240510/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_unused.h` & `libvmdk-20240510/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_wide_split_string.h` & `libvmdk-20240510/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_error.c` & `libvmdk-20240510/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_narrow_split_string.c` & `libvmdk-20240510/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_extern.h` & `libvmdk-20240510/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_error.h` & `libvmdk-20240510/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_support.c` & `libvmdk-20240510/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_wide_string.h` & `libvmdk-20240510/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/Makefile.in` & `libvmdk-20240510/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -458,14 +458,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -522,16 +524,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -540,15 +542,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -753,24 +756,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -859,17 +870,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcsplit/libcsplit_narrow_split_string.h` & `libvmdk-20240510/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcsplit/libcsplit_narrow_string.h` & `libvmdk-20240510/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/remove-potcdate.sin` & `libvmdk-20240510/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/Makefile.in.in` & `libvmdk-20240510/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/en@quot.header` & `libvmdk-20240510/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/en@boldquot.header` & `libvmdk-20240510/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/insert-header.sin` & `libvmdk-20240510/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/Makevars` & `libvmdk-20240510/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/Makevars.in` & `libvmdk-20240510/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/po/Rules-quot` & `libvmdk-20240510/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1251.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf16_string.c` & `libvmdk-20240510/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base16_stream.c` & `libvmdk-20240510/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf8_stream.h` & `libvmdk-20240510/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_2.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_932.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_dingbats.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf8_string.c` & `libvmdk-20240510/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base64_stream.c` & `libvmdk-20240510/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_error.h` & `libvmdk-20240510/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_turkish.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_unicode_character.c` & `libvmdk-20240510/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_gaelic.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_arabic.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_thai.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_874.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_15.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf8_string.h` & `libvmdk-20240510/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_16.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1255.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf7_stream.c` & `libvmdk-20240510/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_byte_stream.h` & `libvmdk-20240510/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_koi8_u.c` & `libvmdk-20240510/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_unused.h` & `libvmdk-20240510/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_6.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_14.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base64_stream.h` & `libvmdk-20240510/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_error.c` & `libvmdk-20240510/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_centraleurroman.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_romanian.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_6.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_9.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_russian.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_dingbats.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_15.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_936.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_croatian.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_scsu.h` & `libvmdk-20240510/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/Makefile.am` & `libvmdk-20240510/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libvmdk-20240303/libuna/libuna_utf32_stream.c` & `libvmdk-20240510/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_936.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_10.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_roman.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf7_stream.h` & `libvmdk-20240510/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_3.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_thai.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_farsi.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_ukrainian.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_inuit.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_932.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_874.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_5.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_10.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_definitions.h` & `libvmdk-20240510/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libvmdk-20240303/libuna/libuna_url_stream.h` & `libvmdk-20240510/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_icelandic.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_koi8_u.h` & `libvmdk-20240510/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf16_stream.c` & `libvmdk-20240510/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1253.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_4.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_greek.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_libcerror.h` & `libvmdk-20240510/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_centraleurroman.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1254.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_13.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_7.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1255.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_unicode_character.h` & `libvmdk-20240510/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_8.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_13.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_949.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_cyrillic.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_celtic.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_support.h` & `libvmdk-20240510/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_4.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_949.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf16_stream.h` & `libvmdk-20240510/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_symbol.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_roman.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1257.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1254.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_950.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_extern.h` & `libvmdk-20240510/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1256.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_types.h` & `libvmdk-20240510/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base32_stream.h` & `libvmdk-20240510/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1253.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_16.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf8_stream.c` & `libvmdk-20240510/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1250.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_2.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_support.c` & `libvmdk-20240510/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_koi8_r.c` & `libvmdk-20240510/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_5.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf16_string.h` & `libvmdk-20240510/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf32_string.c` & `libvmdk-20240510/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_icelandic.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1256.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf32_string.h` & `libvmdk-20240510/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_romanian.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_8.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_koi8_r.h` & `libvmdk-20240510/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_cyrillic.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_arabic.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_croatian.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_9.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_greek.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1258.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_7.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/Makefile.in` & `libvmdk-20240510/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -626,14 +626,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -690,16 +692,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -765,15 +767,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1035,24 +1038,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1198,17 +1266,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_3.c` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1250.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_scsu.c` & `libvmdk-20240510/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1252.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_turkish.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_ukrainian.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_russian.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1258.c` & `libvmdk-20240510/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_celtic.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_byte_stream.c` & `libvmdk-20240510/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_gaelic.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_utf32_stream.h` & `libvmdk-20240510/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_symbol.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1257.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_inuit.h` & `libvmdk-20240510/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_mac_farsi.c` & `libvmdk-20240510/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_950.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_url_stream.c` & `libvmdk-20240510/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1251.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_windows_1252.h` & `libvmdk-20240510/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_codepage_iso_8859_14.h` & `libvmdk-20240510/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base16_stream.h` & `libvmdk-20240510/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libuna/libuna_base32_stream.c` & `libvmdk-20240510/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/Makefile.in` & `libvmdk-20240510/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -508,14 +508,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -634,16 +636,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvmdk.pc \
+	libvmdk.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libvmdk.pc
 
 all: all-recursive
 
@@ -1060,23 +1069,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1187,22 +1199,10 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvmdk && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvmdk.pc
-	-rm -f libvmdk.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvmdk-20240303/libfvalue/libfvalue_filetime.c` & `libvmdk-20240510/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_utf16_string.c` & `libvmdk-20240510/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libfwnt.h` & `libvmdk-20240510/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value.c` & `libvmdk-20240510/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value.h` & `libvmdk-20240510/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_definitions.h` & `libvmdk-20240510/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libvmdk-20240303/libfvalue/libfvalue_codepage.h` & `libvmdk-20240510/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_split_utf16_string.c` & `libvmdk-20240510/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_error.c` & `libvmdk-20240510/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_utf8_string.c` & `libvmdk-20240510/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_unused.h` & `libvmdk-20240510/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_split_utf16_string.h` & `libvmdk-20240510/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_filetime.h` & `libvmdk-20240510/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_support.c` & `libvmdk-20240510/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_extern.h` & `libvmdk-20240510/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/Makefile.am` & `libvmdk-20240510/libfvalue/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -38,19 +38,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value_type.h` & `libvmdk-20240510/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libcerror.h` & `libvmdk-20240510/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_split_utf8_string.c` & `libvmdk-20240510/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_data_handle.h` & `libvmdk-20240510/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libcnotify.h` & `libvmdk-20240510/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_data_handle.c` & `libvmdk-20240510/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_integer.c` & `libvmdk-20240510/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value_type.c` & `libvmdk-20240510/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_integer.h` & `libvmdk-20240510/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_binary_data.h` & `libvmdk-20240510/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value_entry.h` & `libvmdk-20240510/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_utf16_string.h` & `libvmdk-20240510/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_error.h` & `libvmdk-20240510/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_table.h` & `libvmdk-20240510/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libfguid.h` & `libvmdk-20240510/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_split_utf8_string.h` & `libvmdk-20240510/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_floating_point.h` & `libvmdk-20240510/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libfdatetime.h` & `libvmdk-20240510/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_string.h` & `libvmdk-20240510/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_binary_data.c` & `libvmdk-20240510/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_value_entry.c` & `libvmdk-20240510/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libcdata.h` & `libvmdk-20240510/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_support.h` & `libvmdk-20240510/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_table.c` & `libvmdk-20240510/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/Makefile.in` & `libvmdk-20240510/libfvalue/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -489,14 +489,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -553,16 +555,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -593,15 +595,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -816,24 +819,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -932,17 +953,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libfvalue/libfvalue_utf8_string.h` & `libvmdk-20240510/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_floating_point.c` & `libvmdk-20240510/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_types.h` & `libvmdk-20240510/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_string.c` & `libvmdk-20240510/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libfvalue/libfvalue_libuna.h` & `libvmdk-20240510/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_definitions.h` & `libvmdk-20240510/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libvmdk-20240303/libcnotify/libcnotify_extern.h` & `libvmdk-20240510/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_support.c` & `libvmdk-20240510/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_stream.h` & `libvmdk-20240510/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/Makefile.am` & `libvmdk-20240510/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcnotify/libcnotify_unused.h` & `libvmdk-20240510/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_verbose.h` & `libvmdk-20240510/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_print.h` & `libvmdk-20240510/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_stream.c` & `libvmdk-20240510/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_support.h` & `libvmdk-20240510/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_verbose.c` & `libvmdk-20240510/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/Makefile.in` & `libvmdk-20240510/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -450,14 +450,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -514,30 +516,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -740,24 +743,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -844,17 +853,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libcnotify/libcnotify_libcerror.h` & `libvmdk-20240510/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcnotify/libcnotify_print.c` & `libvmdk-20240510/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk.rc` & `libvmdk-20240510/libvmdk/libvmdk.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the VMware Virtual Disk (VMDK) format\0"
-      VALUE "FileVersion",		"20240303" "\0"
+      VALUE "FileVersion",		"20240510" "\0"
       VALUE "InternalName",		"libvmdk.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvmdk.dll\0"
       VALUE "ProductName",		"libvmdk\0"
-      VALUE "ProductVersion",		"20240303" "\0"
+      VALUE "ProductVersion",		"20240510" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvmdk/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcpath.h` & `libvmdk-20240510/libvmdk/libvmdk_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_definitions.h.in` & `libvmdk-20240510/libvmdk/libvmdk_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_bit_stream.h` & `libvmdk-20240510/libvmdk/libvmdk_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_support.c` & `libvmdk-20240510/libvmdk/libvmdk_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_huffman_tree.h` & `libvmdk-20240510/libvmdk/libvmdk_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_table.c` & `libvmdk-20240510/libvmdk/libvmdk_extent_table.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_deflate.c` & `libvmdk-20240510/libvmdk/libvmdk_deflate.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcdata.h` & `libvmdk-20240510/libvmdk/libvmdk_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_error.c` & `libvmdk-20240510/libvmdk/libvmdk_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk.rc.in` & `libvmdk-20240510/libvmdk/libvmdk.rc.in`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_data.h` & `libvmdk-20240510/libvmdk/libvmdk_grain_data.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_huffman_tree.c` & `libvmdk-20240510/libvmdk/libvmdk_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_group.c` & `libvmdk-20240510/libvmdk/libvmdk_grain_group.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libuna.h` & `libvmdk-20240510/libvmdk/libvmdk_libuna.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_system_string.c` & `libvmdk-20240510/libvmdk/libvmdk_system_string.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_handle.c` & `libvmdk-20240510/libvmdk/libvmdk_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_support.h` & `libvmdk-20240510/libvmdk/libvmdk_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libbfio.h` & `libvmdk-20240510/libvmdk/libvmdk_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/Makefile.am` & `libvmdk-20240510/libvmdk/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -82,18 +82,19 @@
 libvmdk_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libvmdk_definitions.h.in \
 	libvmdk.rc \
 	libvmdk.rc.in
 
-distclean: clean
-	-rm -f libvmdk_definitions.h
-	-rm -f libvmdk.rc
-	-rm -f Makefile
+DISTCLEANFILES = \
+	libvmdk_definitions.h \
+	libvmdk.rc \
+	Makefile \
+	Makefile.in
 
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvmdk ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvmdk_la_SOURCES)
```

### Comparing `libvmdk-20240303/libvmdk/libvmdk_definitions.h` & `libvmdk-20240510/libvmdk/libvmdk_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBVMDK )
 #include <libvmdk/definitions.h>
 
 /* The definitions in <libvmdk/definitions.h> are copied here
  * for local use of libvmdk
  */
 #else
-#define LIBVMDK_VERSION						20240303
+#define LIBVMDK_VERSION						20240510
 
 /* The libvmdk version string
  */
-#define LIBVMDK_VERSION_STRING					"20240303"
+#define LIBVMDK_VERSION_STRING					"20240510"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVMDK_ACCESS_FLAGS
```

### Comparing `libvmdk-20240303/libvmdk/vmdk_sparse_file_header.h` & `libvmdk-20240510/libvmdk/vmdk_sparse_file_header.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_descriptor.c` & `libvmdk-20240510/libvmdk/libvmdk_extent_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_debug.c` & `libvmdk-20240510/libvmdk/libvmdk_debug.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libfvalue.h` & `libvmdk-20240510/libvmdk/libvmdk_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_table.c` & `libvmdk-20240510/libvmdk/libvmdk_grain_table.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcerror.h` & `libvmdk-20240510/libvmdk/libvmdk_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_deflate.h` & `libvmdk-20240510/libvmdk/libvmdk_deflate.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_group.h` & `libvmdk-20240510/libvmdk/libvmdk_grain_group.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcnotify.h` & `libvmdk-20240510/libvmdk/libvmdk_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_io_handle.c` & `libvmdk-20240510/libvmdk/libvmdk_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcfile.h` & `libvmdk-20240510/libvmdk/libvmdk_libcfile.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcsplit.h` & `libvmdk-20240510/libvmdk/libvmdk_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_table.h` & `libvmdk-20240510/libvmdk/libvmdk_grain_table.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_error.h` & `libvmdk-20240510/libvmdk/libvmdk_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_unused.h` & `libvmdk-20240510/libvmdk/libvmdk_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_file.h` & `libvmdk-20240510/libvmdk/libvmdk_extent_file.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_notify.c` & `libvmdk-20240510/libvmdk/libvmdk_notify.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_io_handle.h` & `libvmdk-20240510/libvmdk/libvmdk_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_descriptor.h` & `libvmdk-20240510/libvmdk/libvmdk_extent_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libfdata.h` & `libvmdk-20240510/libvmdk/libvmdk_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk.c` & `libvmdk-20240510/libvmdk/libvmdk.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_table.h` & `libvmdk-20240510/libvmdk/libvmdk_extent_table.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_compression.h` & `libvmdk-20240510/libvmdk/libvmdk_compression.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_grain_data.c` & `libvmdk-20240510/libvmdk/libvmdk_grain_data.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_system_string.h` & `libvmdk-20240510/libvmdk/libvmdk_system_string.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_debug.h` & `libvmdk-20240510/libvmdk/libvmdk_debug.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/cowd_sparse_file_header.h` & `libvmdk-20240510/libvmdk/cowd_sparse_file_header.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_notify.h` & `libvmdk-20240510/libvmdk/libvmdk_notify.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libclocale.h` & `libvmdk-20240510/libvmdk/libvmdk_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_handle.h` & `libvmdk-20240510/libvmdk/libvmdk_handle.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_file.c` & `libvmdk-20240510/libvmdk/libvmdk_extent_file.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extern.h` & `libvmdk-20240510/libvmdk/libvmdk_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_descriptor_file.c` & `libvmdk-20240510/libvmdk/libvmdk_descriptor_file.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/Makefile.in` & `libvmdk-20240510/libvmdk/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -494,14 +494,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -559,16 +561,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -643,14 +645,20 @@
 
 libvmdk_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libvmdk_definitions.h.in \
 	libvmdk.rc \
 	libvmdk.rc.in
 
+DISTCLEANFILES = \
+	libvmdk_definitions.h \
+	libvmdk.rc \
+	Makefile \
+	Makefile.in
+
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
 	  case '$(am__configure_deps)' in \
@@ -898,23 +906,46 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libvmdk.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_compression.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_debug.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_deflate.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_descriptor_file.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_error.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_extent_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_extent_file.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_extent_table.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_extent_values.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_grain_data.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_grain_group.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_grain_table.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_handle.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_notify.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_support.Plo
+	-rm -f ./$(DEPDIR)/libvmdk_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1017,19 +1048,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvmdk_definitions.h
-	-rm -f libvmdk.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvmdk ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvmdk_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/libvmdk/libvmdk_bit_stream.c` & `libvmdk-20240510/libvmdk/libvmdk_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_values.c` & `libvmdk-20240510/libvmdk/libvmdk_extent_values.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libcthreads.h` & `libvmdk-20240510/libvmdk/libvmdk_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_types.h` & `libvmdk-20240510/libvmdk/libvmdk_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_extent_values.h` & `libvmdk-20240510/libvmdk/libvmdk_extent_values.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_descriptor_file.h` & `libvmdk-20240510/libvmdk/libvmdk_descriptor_file.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_compression.c` & `libvmdk-20240510/libvmdk/libvmdk_compression.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libvmdk/libvmdk_libfcache.h` & `libvmdk-20240510/libvmdk/libvmdk_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_system.c` & `libvmdk-20240510/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_error.c` & `libvmdk-20240510/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_extern.h` & `libvmdk-20240510/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/Makefile.am` & `libvmdk-20240510/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libvmdk-20240303/libcerror/libcerror_types.h` & `libvmdk-20240510/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_support.h` & `libvmdk-20240510/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_error.h` & `libvmdk-20240510/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_system.h` & `libvmdk-20240510/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_definitions.h` & `libvmdk-20240510/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libvmdk-20240303/libcerror/libcerror_support.c` & `libvmdk-20240510/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/libcerror_unused.h` & `libvmdk-20240510/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/libcerror/Makefile.in` & `libvmdk-20240510/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -511,28 +513,29 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -734,24 +737,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -837,17 +845,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvmdk-20240303/aclocal.m4` & `libvmdk-20240510/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvmdk-20240303/configure.ac` & `libvmdk-20240510/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvmdk],
- [20240303],
+ [20240510],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvmdk.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

