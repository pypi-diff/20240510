# Comparing `tmp/advanced_navigation-0.1.4.tar.gz` & `tmp/advanced_navigation-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_navigation-0.1.4.tar", max compression
+gzip compressed data, was "advanced_navigation-0.1.41.tar", max compression
```

## Comparing `advanced_navigation-0.1.4.tar` & `advanced_navigation-0.1.41.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1080 2024-03-21 02:22:47.322594 advanced_navigation-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1249 2024-04-11 05:29:01.828944 advanced_navigation-0.1.4/README.md
--rw-r--r--   0        0        0       59 2024-05-10 01:28:43.535786 advanced_navigation-0.1.4/advanced_navigation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 01:28:50.495778 advanced_navigation-0.1.4/advanced_navigation/an_devices/__init__.py
--rw-r--r--   0        0        0     4977 2024-03-21 02:22:47.322594 advanced_navigation-0.1.4/advanced_navigation/an_devices/advanced_navigation_device_serial.py
--rw-r--r--   0        0        0     4591 2024-04-11 05:29:04.880960 advanced_navigation-0.1.4/advanced_navigation/an_devices/advanced_navigation_device_tcp.py
--rw-r--r--   0        0        0     2886 2024-03-27 02:21:48.013115 advanced_navigation-0.1.4/advanced_navigation/an_devices/air_data_unit_device.py
--rw-r--r--   0        0        0     4049 2024-03-27 02:21:48.013115 advanced_navigation-0.1.4/advanced_navigation/an_devices/boreas_device.py
--rw-r--r--   0        0        0     5928 2024-04-11 05:29:11.484996 advanced_navigation-0.1.4/advanced_navigation/an_devices/certus_device.py
--rw-r--r--   0        0        0     4091 2024-04-11 05:29:06.596969 advanced_navigation-0.1.4/advanced_navigation/an_devices/certus_evo_device.py
--rw-r--r--   0        0        0     3651 2024-03-27 02:21:48.017115 advanced_navigation-0.1.4/advanced_navigation/an_devices/gnss_compass_device.py
--rw-r--r--   0        0        0     3702 2024-03-27 02:21:48.017115 advanced_navigation-0.1.4/advanced_navigation/an_devices/motus_device.py
--rw-r--r--   0        0        0     3525 2024-03-27 02:21:48.021115 advanced_navigation-0.1.4/advanced_navigation/an_devices/orientus_device.py
--rw-r--r--   0        0        0     4383 2024-03-27 02:21:48.021115 advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_device.py
--rw-r--r--   0        0        0     3800 2024-03-27 02:21:48.021115 advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_dual_device.py
--rw-r--r--   0        0        0     3727 2024-03-27 02:21:48.021115 advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_fog_device.py
--rw-r--r--   0        0        0     3790 2024-03-27 02:21:48.021115 advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_fog_dual_device.py
--rw-r--r--   0        0        0     2391 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/__init__.py
--rw-r--r--   0        0        0     3448 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_0.py
--rw-r--r--   0        0        0     3133 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_1.py
--rw-r--r--   0        0        0     3561 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_10.py
--rw-r--r--   0        0        0     4701 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_11.py
--rw-r--r--   0        0        0     3651 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_13.py
--rw-r--r--   0        0        0     4126 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_14.py
--rw-r--r--   0        0        0     3514 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_180.py
--rw-r--r--   0        0        0     4571 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_181.py
--rw-r--r--   0        0        0     3603 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_182.py
--rw-r--r--   0        0        0     4525 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_184.py
--rw-r--r--   0        0        0     4323 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_185.py
--rw-r--r--   0        0        0     4875 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_186.py
--rw-r--r--   0        0        0     8383 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_188.py
--rw-r--r--   0        0        0     3882 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_189.py
--rw-r--r--   0        0        0     3226 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_190.py
--rw-r--r--   0        0        0     3814 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_191.py
--rw-r--r--   0        0        0     3583 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_192.py
--rw-r--r--   0        0        0     2982 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_193.py
--rw-r--r--   0        0        0     4217 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_194.py
--rw-r--r--   0        0        0    11666 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_195.py
--rw-r--r--   0        0        0     4447 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_196.py
--rw-r--r--   0        0        0     9396 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_197.py
--rw-r--r--   0        0        0     3160 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_198.py
--rw-r--r--   0        0        0     3474 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_199.py
--rw-r--r--   0        0        0     3363 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_2.py
--rw-r--r--   0        0        0     7843 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_20.py
--rw-r--r--   0        0        0     4257 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_202.py
--rw-r--r--   0        0        0     3746 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_203.py
--rw-r--r--   0        0        0     3022 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_21.py
--rw-r--r--   0        0        0     3392 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_22.py
--rw-r--r--   0        0        0     3209 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_23.py
--rw-r--r--   0        0        0     3130 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_24.py
--rw-r--r--   0        0        0     3130 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_25.py
--rw-r--r--   0        0        0     3165 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_26.py
--rw-r--r--   0        0        0     3189 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_27.py
--rw-r--r--   0        0        0     5561 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_28.py
--rw-r--r--   0        0        0     7159 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_29.py
--rw-r--r--   0        0        0     3857 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_3.py
--rw-r--r--   0        0        0     3361 2024-03-21 02:22:47.326594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_30.py
--rw-r--r--   0        0        0     5077 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_31.py
--rw-r--r--   0        0        0     3057 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_32.py
--rw-r--r--   0        0        0     3041 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_33.py
--rw-r--r--   0        0        0     3191 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_34.py
--rw-r--r--   0        0        0     3037 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_35.py
--rw-r--r--   0        0        0     3041 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_36.py
--rw-r--r--   0        0        0     3046 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_37.py
--rw-r--r--   0        0        0     3129 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_38.py
--rw-r--r--   0        0        0     3063 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_39.py
--rw-r--r--   0        0        0     2918 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_4.py
--rw-r--r--   0        0        0     3087 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_40.py
--rw-r--r--   0        0        0     3197 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_41.py
--rw-r--r--   0        0        0     3069 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_42.py
--rw-r--r--   0        0        0     3137 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_43.py
--rw-r--r--   0        0        0     4058 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_44.py
--rw-r--r--   0        0        0     3565 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_45.py
--rw-r--r--   0        0        0     3564 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_46.py
--rw-r--r--   0        0        0     3938 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_47.py
--rw-r--r--   0        0        0     3353 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_48.py
--rw-r--r--   0        0        0     3014 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_49.py
--rw-r--r--   0        0        0     3035 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_5.py
--rw-r--r--   0        0        0     3080 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_50.py
--rw-r--r--   0        0        0     3215 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_51.py
--rw-r--r--   0        0        0     3346 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_52.py
--rw-r--r--   0        0        0     3337 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_53.py
--rw-r--r--   0        0        0     2951 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_54.py
--rw-r--r--   0        0        0     2996 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_55.py
--rw-r--r--   0        0        0     3433 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_57.py
--rw-r--r--   0        0        0     3155 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_58.py
--rw-r--r--   0        0        0     7729 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_60.py
--rw-r--r--   0        0        0    10031 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_61.py
--rw-r--r--   0        0        0     4048 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_67.py
--rw-r--r--   0        0        0     6885 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_68.py
--rw-r--r--   0        0        0     6986 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_69.py
--rw-r--r--   0        0        0     3683 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_7.py
--rw-r--r--   0        0        0     4560 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_70.py
--rw-r--r--   0        0        0     5421 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_71.py
--rw-r--r--   0        0        0     3239 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_72.py
--rw-r--r--   0        0        0     3275 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_73.py
--rw-r--r--   0        0        0     3977 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_75.py
--rw-r--r--   0        0        0     3685 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_8.py
--rw-r--r--   0        0        0     3641 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_80.py
--rw-r--r--   0        0        0     2899 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_83.py
--rw-r--r--   0        0        0     4886 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_84.py
--rw-r--r--   0        0        0     3521 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_85.py
--rw-r--r--   0        0        0     2992 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_86.py
--rw-r--r--   0        0        0     3019 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_9.py
--rw-r--r--   0        0        0     9230 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_protocol.py
--rw-r--r--   0        0        0     4857 2024-03-21 02:22:47.330594 advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packets.py
--rw-r--r--   0        0        0      404 2024-05-10 01:29:18.519742 advanced_navigation-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 advanced_navigation-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-21 02:22:47.322594 advanced_navigation-0.1.41/LICENSE.txt
+-rw-r--r--   0        0        0     1249 2024-04-11 05:29:01.828944 advanced_navigation-0.1.41/README.md
+-rw-r--r--   0        0        0       41 2024-05-10 01:31:24.399645 advanced_navigation-0.1.41/advanced_navigation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 01:34:55.951767 advanced_navigation-0.1.41/advanced_navigation/an_devices/__init__.py
+-rw-r--r--   0        0        0     4977 2024-03-21 02:22:47.322594 advanced_navigation-0.1.41/advanced_navigation/an_devices/advanced_navigation_device_serial.py
+-rw-r--r--   0        0        0     4591 2024-04-11 05:29:04.880960 advanced_navigation-0.1.41/advanced_navigation/an_devices/advanced_navigation_device_tcp.py
+-rw-r--r--   0        0        0     2886 2024-03-27 02:21:48.013115 advanced_navigation-0.1.41/advanced_navigation/an_devices/air_data_unit_device.py
+-rw-r--r--   0        0        0     4049 2024-03-27 02:21:48.013115 advanced_navigation-0.1.41/advanced_navigation/an_devices/boreas_device.py
+-rw-r--r--   0        0        0     5928 2024-04-11 05:29:11.484996 advanced_navigation-0.1.41/advanced_navigation/an_devices/certus_device.py
+-rw-r--r--   0        0        0     4091 2024-04-11 05:29:06.596969 advanced_navigation-0.1.41/advanced_navigation/an_devices/certus_evo_device.py
+-rw-r--r--   0        0        0     3651 2024-03-27 02:21:48.017115 advanced_navigation-0.1.41/advanced_navigation/an_devices/gnss_compass_device.py
+-rw-r--r--   0        0        0     3702 2024-03-27 02:21:48.017115 advanced_navigation-0.1.41/advanced_navigation/an_devices/motus_device.py
+-rw-r--r--   0        0        0     3525 2024-03-27 02:21:48.021115 advanced_navigation-0.1.41/advanced_navigation/an_devices/orientus_device.py
+-rw-r--r--   0        0        0     4383 2024-03-27 02:21:48.021115 advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_device.py
+-rw-r--r--   0        0        0     3800 2024-03-27 02:21:48.021115 advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_dual_device.py
+-rw-r--r--   0        0        0     3727 2024-03-27 02:21:48.021115 advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_fog_device.py
+-rw-r--r--   0        0        0     3790 2024-03-27 02:21:48.021115 advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_fog_dual_device.py
+-rw-r--r--   0        0        0     2391 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/__init__.py
+-rw-r--r--   0        0        0     3448 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_0.py
+-rw-r--r--   0        0        0     3133 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_1.py
+-rw-r--r--   0        0        0     3561 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_10.py
+-rw-r--r--   0        0        0     4701 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_11.py
+-rw-r--r--   0        0        0     3651 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_13.py
+-rw-r--r--   0        0        0     4126 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_14.py
+-rw-r--r--   0        0        0     3514 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_180.py
+-rw-r--r--   0        0        0     4571 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_181.py
+-rw-r--r--   0        0        0     3603 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_182.py
+-rw-r--r--   0        0        0     4525 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_184.py
+-rw-r--r--   0        0        0     4323 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_185.py
+-rw-r--r--   0        0        0     4875 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_186.py
+-rw-r--r--   0        0        0     8383 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_188.py
+-rw-r--r--   0        0        0     3882 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_189.py
+-rw-r--r--   0        0        0     3226 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_190.py
+-rw-r--r--   0        0        0     3814 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_191.py
+-rw-r--r--   0        0        0     3583 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_192.py
+-rw-r--r--   0        0        0     2982 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_193.py
+-rw-r--r--   0        0        0     4217 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_194.py
+-rw-r--r--   0        0        0    11666 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_195.py
+-rw-r--r--   0        0        0     4447 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_196.py
+-rw-r--r--   0        0        0     9396 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_197.py
+-rw-r--r--   0        0        0     3160 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_198.py
+-rw-r--r--   0        0        0     3474 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_199.py
+-rw-r--r--   0        0        0     3363 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_2.py
+-rw-r--r--   0        0        0     7843 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_20.py
+-rw-r--r--   0        0        0     4257 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_202.py
+-rw-r--r--   0        0        0     3746 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_203.py
+-rw-r--r--   0        0        0     3022 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_21.py
+-rw-r--r--   0        0        0     3392 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_22.py
+-rw-r--r--   0        0        0     3209 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_23.py
+-rw-r--r--   0        0        0     3130 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_24.py
+-rw-r--r--   0        0        0     3130 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_25.py
+-rw-r--r--   0        0        0     3165 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_26.py
+-rw-r--r--   0        0        0     3189 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_27.py
+-rw-r--r--   0        0        0     5561 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_28.py
+-rw-r--r--   0        0        0     7159 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_29.py
+-rw-r--r--   0        0        0     3857 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_3.py
+-rw-r--r--   0        0        0     3361 2024-03-21 02:22:47.326594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_30.py
+-rw-r--r--   0        0        0     5077 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_31.py
+-rw-r--r--   0        0        0     3057 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_32.py
+-rw-r--r--   0        0        0     3041 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_33.py
+-rw-r--r--   0        0        0     3191 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_34.py
+-rw-r--r--   0        0        0     3037 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_35.py
+-rw-r--r--   0        0        0     3041 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_36.py
+-rw-r--r--   0        0        0     3046 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_37.py
+-rw-r--r--   0        0        0     3129 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_38.py
+-rw-r--r--   0        0        0     3063 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_39.py
+-rw-r--r--   0        0        0     2918 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_4.py
+-rw-r--r--   0        0        0     3087 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_40.py
+-rw-r--r--   0        0        0     3197 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_41.py
+-rw-r--r--   0        0        0     3069 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_42.py
+-rw-r--r--   0        0        0     3137 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_43.py
+-rw-r--r--   0        0        0     4058 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_44.py
+-rw-r--r--   0        0        0     3565 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_45.py
+-rw-r--r--   0        0        0     3564 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_46.py
+-rw-r--r--   0        0        0     3938 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_47.py
+-rw-r--r--   0        0        0     3353 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_48.py
+-rw-r--r--   0        0        0     3014 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_49.py
+-rw-r--r--   0        0        0     3035 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_5.py
+-rw-r--r--   0        0        0     3080 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_50.py
+-rw-r--r--   0        0        0     3215 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_51.py
+-rw-r--r--   0        0        0     3346 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_52.py
+-rw-r--r--   0        0        0     3337 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_53.py
+-rw-r--r--   0        0        0     2951 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_54.py
+-rw-r--r--   0        0        0     2996 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_55.py
+-rw-r--r--   0        0        0     3433 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_57.py
+-rw-r--r--   0        0        0     3155 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_58.py
+-rw-r--r--   0        0        0     7729 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_60.py
+-rw-r--r--   0        0        0    10031 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_61.py
+-rw-r--r--   0        0        0     4048 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_67.py
+-rw-r--r--   0        0        0     6885 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_68.py
+-rw-r--r--   0        0        0     6986 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_69.py
+-rw-r--r--   0        0        0     3683 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_7.py
+-rw-r--r--   0        0        0     4560 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_70.py
+-rw-r--r--   0        0        0     5421 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_71.py
+-rw-r--r--   0        0        0     3239 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_72.py
+-rw-r--r--   0        0        0     3275 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_73.py
+-rw-r--r--   0        0        0     3977 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_75.py
+-rw-r--r--   0        0        0     3685 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_8.py
+-rw-r--r--   0        0        0     3641 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_80.py
+-rw-r--r--   0        0        0     2899 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_83.py
+-rw-r--r--   0        0        0     4886 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_84.py
+-rw-r--r--   0        0        0     3521 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_85.py
+-rw-r--r--   0        0        0     2992 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_86.py
+-rw-r--r--   0        0        0     3019 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_9.py
+-rw-r--r--   0        0        0     9230 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_protocol.py
+-rw-r--r--   0        0        0     4857 2024-03-21 02:22:47.330594 advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packets.py
+-rw-r--r--   0        0        0      405 2024-05-10 01:35:16.460092 advanced_navigation-0.1.41/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 advanced_navigation-0.1.41/PKG-INFO
```

### Comparing `advanced_navigation-0.1.4/LICENSE.txt` & `advanced_navigation-0.1.41/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/README.md` & `advanced_navigation-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/advanced_navigation_device_serial.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/advanced_navigation_device_serial.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/advanced_navigation_device_tcp.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/advanced_navigation_device_tcp.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/air_data_unit_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/air_data_unit_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/boreas_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/boreas_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/certus_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/certus_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/certus_evo_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/certus_evo_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/gnss_compass_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/gnss_compass_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/motus_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/motus_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/orientus_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/orientus_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_dual_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_dual_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_fog_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_fog_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/an_devices/spatial_fog_dual_device.py` & `advanced_navigation-0.1.41/advanced_navigation/an_devices/spatial_fog_dual_device.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/__init__.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_0.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_0.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_1.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_1.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_10.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_10.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_11.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_11.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_13.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_13.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_14.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_14.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_180.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_180.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_181.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_181.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_182.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_182.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_184.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_184.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_185.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_185.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_186.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_186.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_188.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_188.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_189.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_189.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_190.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_190.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_191.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_191.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_192.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_192.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_193.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_193.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_194.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_194.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_195.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_195.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_196.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_196.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_197.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_197.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_198.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_198.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_199.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_199.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_2.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_2.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_20.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_20.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_202.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_202.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_203.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_203.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_21.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_21.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_22.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_22.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_23.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_23.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_24.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_24.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_25.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_25.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_26.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_26.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_27.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_27.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_28.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_28.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_29.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_29.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_3.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_3.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_30.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_30.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_31.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_31.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_32.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_32.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_33.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_33.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_34.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_34.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_35.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_35.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_36.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_36.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_37.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_37.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_38.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_38.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_39.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_39.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_4.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_4.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_40.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_40.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_41.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_41.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_42.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_42.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_43.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_43.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_44.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_44.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_45.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_45.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_46.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_46.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_47.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_47.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_48.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_48.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_49.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_49.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_5.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_5.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_50.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_50.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_51.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_51.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_52.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_52.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_53.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_53.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_54.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_54.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_55.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_55.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_57.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_57.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_58.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_58.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_60.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_60.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_61.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_61.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_67.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_67.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_68.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_68.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_69.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_69.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_7.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_7.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_70.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_70.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_71.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_71.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_72.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_72.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_73.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_73.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_75.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_75.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_8.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_8.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_80.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_80.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_83.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_83.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_84.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_84.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_85.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_85.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_86.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_86.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_9.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_9.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packet_protocol.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packet_protocol.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/advanced_navigation/anpp_packets/an_packets.py` & `advanced_navigation-0.1.41/advanced_navigation/anpp_packets/an_packets.py`

 * *Files identical despite different names*

### Comparing `advanced_navigation-0.1.4/PKG-INFO` & `advanced_navigation-0.1.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced_navigation
-Version: 0.1.4
+Version: 0.1.41
 Summary: 
 Author: Charles Balderstone
 Author-email: charles.balderstone@advancednavigation.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

