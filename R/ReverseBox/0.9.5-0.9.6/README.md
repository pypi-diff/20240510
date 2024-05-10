# Comparing `tmp/ReverseBox-0.9.5.tar.gz` & `tmp/ReverseBox-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.9.5.tar", last modified: Mon May  6 16:04:03 2024, max compression
+gzip compressed data, was "ReverseBox-0.9.6.tar", last modified: Fri May 10 15:26:03 2024, max compression
```

## Comparing `ReverseBox-0.9.5.tar` & `ReverseBox-0.9.6.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.682160 ReverseBox-0.9.5/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     6982 2024-05-06 16:04:03.681163 ReverseBox-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     5581 2024-05-03 23:01:57.000000 ReverseBox-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.625312 ReverseBox-0.9.5/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     6982 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.626309 ReverseBox-0.9.5/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.9.5/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.630299 ReverseBox-0.9.5/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.5/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.9.5/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.9.5/reversebox/checksum/checksum_bsd16.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.9.5/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.9.5/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.633291 ReverseBox-0.9.5/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.9.5/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.9.5/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.9.5/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.637280 ReverseBox-0.9.5/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.5/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.9.5/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.9.5/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0     2188 2024-05-06 16:03:40.000000 ReverseBox-0.9.5/reversebox/compression/compression_refpack.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.9.5/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.647253 ReverseBox-0.9.5/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.9.5/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.9.5/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.9.5/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.9.5/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.9.5/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.9.5/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.9.5/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.9.5/reversebox/crc/crc32_asobo.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.9.5/reversebox/crc/crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.9.5/reversebox/crc/crc64_asobo.py
--rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.9.5/reversebox/crc/crc8.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.652240 ReverseBox-0.9.5/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.5/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.9.5/reversebox/encryption/encryption_rot13.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.9.5/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.9.5/reversebox/encryption/encryption_xor_basic_key_guesser.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.9.5/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.9.5/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.658224 ReverseBox-0.9.5/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.5/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.9.5/reversebox/hash/hash_fnv.py
--rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.9.5/reversebox/hash/hash_md2.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.9.5/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.9.5/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.9.5/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.663211 ReverseBox-0.9.5/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.9.5/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.9.5/reversebox/image/image_dds.py
--rw-rw-rw-   0        0        0    12952 2024-05-06 14:14:06.000000 ReverseBox-0.9.5/reversebox/image/image_decoder.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.9.5/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.9.5/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0      668 2024-05-06 14:13:59.000000 ReverseBox-0.9.5/reversebox/image/image_formats.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.670192 ReverseBox-0.9.5/reversebox/image/swizzling/
--rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.9.5/reversebox/image/swizzling/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_3ds.py
--rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_cmpr.py
--rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_ps2.py
--rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_psp.py
--rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_psvita.py
--rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_switch.py
--rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_xbox.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.676176 ReverseBox-0.9.5/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.5/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.9.5/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 13:01:53.000000 ReverseBox-0.9.5/reversebox/io_files/bytes_helper_functions.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.9.5/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.9.5/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.9.5/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.9.5/reversebox/io_files/translation_text_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:04:03.678171 ReverseBox-0.9.5/reversebox/libs/
--rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.9.5/reversebox/libs/__init__.py
--rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.9.5/reversebox/libs/refpack.dll
--rw-rw-rw-   0        0        0       42 2024-05-06 16:04:03.682160 ReverseBox-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-06 16:04:03.000000 ReverseBox-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.267472 ReverseBox-0.9.6/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0     7090 2024-05-10 15:26:03.266496 ReverseBox-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5689 2024-05-10 15:23:26.000000 ReverseBox-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.205983 ReverseBox-0.9.6/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     7090 2024-05-10 15:26:03.000000 ReverseBox-0.9.6/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2450 2024-05-10 15:26:03.000000 ReverseBox-0.9.6/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:26:03.000000 ReverseBox-0.9.6/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-10 15:26:03.000000 ReverseBox-0.9.6/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 15:26:03.000000 ReverseBox-0.9.6/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.206959 ReverseBox-0.9.6/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.9.6/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.213791 ReverseBox-0.9.6/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.6/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_fletcher32.py
+-rw-rw-rw-   0        0        0      339 2024-05-10 15:23:32.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_sum8.py
+-rw-rw-rw-   0        0        0      420 2024-05-10 14:15:25.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_unix_sum_bsd16.py
+-rw-rw-rw-   0        0        0      543 2024-05-10 15:23:32.000000 ReverseBox-0.9.6/reversebox/checksum/checksum_unix_sum_sysv.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.215743 ReverseBox-0.9.6/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.9.6/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.9.6/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.9.6/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.220623 ReverseBox-0.9.6/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.6/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.9.6/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.9.6/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0     2188 2024-05-06 16:03:40.000000 ReverseBox-0.9.6/reversebox/compression/compression_refpack.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.9.6/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.230383 ReverseBox-0.9.6/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.9.6/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.9.6/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.9.6/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.9.6/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.9.6/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.9.6/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.9.6/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.9.6/reversebox/crc/crc32_asobo.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.9.6/reversebox/crc/crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.9.6/reversebox/crc/crc64_asobo.py
+-rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.9.6/reversebox/crc/crc8.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.235264 ReverseBox-0.9.6/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.6/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.9.6/reversebox/encryption/encryption_rot13.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.9.6/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.9.6/reversebox/encryption/encryption_xor_basic_key_guesser.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.9.6/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.9.6/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.241119 ReverseBox-0.9.6/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.6/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.9.6/reversebox/hash/hash_fnv.py
+-rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.9.6/reversebox/hash/hash_md2.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.9.6/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.9.6/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.9.6/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.246976 ReverseBox-0.9.6/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.9.6/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.9.6/reversebox/image/image_dds.py
+-rw-rw-rw-   0        0        0    12952 2024-05-06 14:14:06.000000 ReverseBox-0.9.6/reversebox/image/image_decoder.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.9.6/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.9.6/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0      668 2024-05-06 14:13:59.000000 ReverseBox-0.9.6/reversebox/image/image_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.253808 ReverseBox-0.9.6/reversebox/image/swizzling/
+-rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.9.6/reversebox/image/swizzling/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_3ds.py
+-rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_cmpr.py
+-rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_ps2.py
+-rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_psp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_psvita.py
+-rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_switch.py
+-rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_xbox.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.260640 ReverseBox-0.9.6/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.6/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.9.6/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 13:01:53.000000 ReverseBox-0.9.6/reversebox/io_files/bytes_helper_functions.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.9.6/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.9.6/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.9.6/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.9.6/reversebox/io_files/translation_text_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:26:03.262615 ReverseBox-0.9.6/reversebox/libs/
+-rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.9.6/reversebox/libs/__init__.py
+-rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.9.6/reversebox/libs/refpack.dll
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:26:03.267472 ReverseBox-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-10 15:23:26.000000 ReverseBox-0.9.6/setup.py
```

### Comparing `ReverseBox-0.9.5/LICENSE` & `ReverseBox-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/PKG-INFO` & `ReverseBox-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.9.5
+Version: 0.9.6
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -53,17 +53,19 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
-  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
+  - Sum8 ✔️
+  - Unix Sum BSD-16 ✔️
+  - Unix Sum SYSV ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
@@ -114,14 +116,16 @@
   - MD2 ✔️ <span style="color:yellow">(wrapper only)</span>
   - MD5 ✔️ <span style="color:yellow">(wrapper only)</span>
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (IN PROGRESS) ❌
+  - Decode RGBA2222 ✔️
+  - Decode RGBX2222 ✔️
   - Decode RGB565 ✔️
   - Decode RGB888 ✔️
   - Decode ARGB4444 ✔️
   - Decode RGBA4444 ✔️
   - Decode XRGB1555 ✔️
   - Decode ABGR1555 ✔️
   - Decode XBGR1555 ✔️
```

### Comparing `ReverseBox-0.9.5/README.md` & `ReverseBox-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
-  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
+  - Sum8 ✔️
+  - Unix Sum BSD-16 ✔️
+  - Unix Sum SYSV ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
@@ -80,14 +82,16 @@
   - MD2 ✔️ <span style="color:yellow">(wrapper only)</span>
   - MD5 ✔️ <span style="color:yellow">(wrapper only)</span>
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (IN PROGRESS) ❌
+  - Decode RGBA2222 ✔️
+  - Decode RGBX2222 ✔️
   - Decode RGB565 ✔️
   - Decode RGB888 ✔️
   - Decode ARGB4444 ✔️
   - Decode RGBA4444 ✔️
   - Decode XRGB1555 ✔️
   - Decode ABGR1555 ✔️
   - Decode XBGR1555 ✔️
```

### Comparing `ReverseBox-0.9.5/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.9.6/ReverseBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.9.5
+Version: 0.9.6
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -53,17 +53,19 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
-  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
+  - Sum8 ✔️
+  - Unix Sum BSD-16 ✔️
+  - Unix Sum SYSV ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
@@ -114,14 +116,16 @@
   - MD2 ✔️ <span style="color:yellow">(wrapper only)</span>
   - MD5 ✔️ <span style="color:yellow">(wrapper only)</span>
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (IN PROGRESS) ❌
+  - Decode RGBA2222 ✔️
+  - Decode RGBX2222 ✔️
   - Decode RGB565 ✔️
   - Decode RGB888 ✔️
   - Decode ARGB4444 ✔️
   - Decode RGBA4444 ✔️
   - Decode XRGB1555 ✔️
   - Decode ABGR1555 ✔️
   - Decode XBGR1555 ✔️
```

### Comparing `ReverseBox-0.9.5/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.9.6/ReverseBox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 ReverseBox.egg-info/SOURCES.txt
 ReverseBox.egg-info/dependency_links.txt
 ReverseBox.egg-info/requires.txt
 ReverseBox.egg-info/top_level.txt
 reversebox/__init__.py
 reversebox/checksum/__init__.py
 reversebox/checksum/checksum_adler32.py
-reversebox/checksum/checksum_bsd16.py
 reversebox/checksum/checksum_fletcher16.py
 reversebox/checksum/checksum_fletcher32.py
+reversebox/checksum/checksum_sum8.py
+reversebox/checksum/checksum_unix_sum_bsd16.py
+reversebox/checksum/checksum_unix_sum_sysv.py
 reversebox/common/__init__.py
 reversebox/common/common.py
 reversebox/common/logger.py
 reversebox/compression/__init__.py
 reversebox/compression/compression_jcalg1.py
 reversebox/compression/compression_lzo.py
 reversebox/compression/compression_refpack.py
```

### Comparing `ReverseBox-0.9.5/reversebox/common/logger.py` & `ReverseBox-0.9.6/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/compression/compression_refpack.py` & `ReverseBox-0.9.6/reversebox/compression/compression_refpack.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_arc.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc16_sick.py` & `ReverseBox-0.9.6/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc32_asobo.py` & `ReverseBox-0.9.6/reversebox/crc/crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.9.6/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc64_asobo.py` & `ReverseBox-0.9.6/reversebox/crc/crc64_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/crc/crc8.py` & `ReverseBox-0.9.6/reversebox/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/encryption/encryption_rot13.py` & `ReverseBox-0.9.6/reversebox/encryption/encryption_rot13.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.9.6/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/encryption/encryption_xor_basic_key_guesser.py` & `ReverseBox-0.9.6/reversebox/encryption/encryption_xor_basic_key_guesser.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.9.6/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.9.6/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/hash/hash_fnv.py` & `ReverseBox-0.9.6/reversebox/hash/hash_fnv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/image_dds.py` & `ReverseBox-0.9.6/reversebox/image/image_dds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/image_decoder.py` & `ReverseBox-0.9.6/reversebox/image/image_decoder.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/image_finder_gui.py` & `ReverseBox-0.9.6/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/image_finder_main.py` & `ReverseBox-0.9.6/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/image_formats.py` & `ReverseBox-0.9.6/reversebox/image/image_formats.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_3ds.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_3ds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_cmpr.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_cmpr.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_ps2.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_ps2.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_psp.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_psp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_psvita.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_psvita.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/image/swizzling/swizzle_switch.py` & `ReverseBox-0.9.6/reversebox/image/swizzling/swizzle_switch.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.9.6/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/bytes_helper_functions.py` & `ReverseBox-0.9.6/reversebox/io_files/bytes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/check_file.py` & `ReverseBox-0.9.6/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/file_handler.py` & `ReverseBox-0.9.6/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/mod_handler.py` & `ReverseBox-0.9.6/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.9.6/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/reversebox/libs/refpack.dll` & `ReverseBox-0.9.6/reversebox/libs/refpack.dll`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.5/setup.py` & `ReverseBox-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.9.5"
+VERSION_NUM = "0.9.6"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

