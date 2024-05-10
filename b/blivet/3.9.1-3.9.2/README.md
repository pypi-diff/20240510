# Comparing `tmp/blivet-3.9.1.tar.gz` & `tmp/blivet-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blivet-3.9.1.tar", last modified: Tue Feb 27 09:53:17 2024, max compression
+gzip compressed data, was "blivet-3.9.2.tar", last modified: Thu Mar 28 12:15:41 2024, max compression
```

## Comparing `blivet-3.9.1.tar` & `blivet-3.9.2.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.121024 blivet-3.9.1/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18092 2024-02-27 09:46:59.000000 blivet-3.9.1/COPYING
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26530 2024-02-27 09:46:59.000000 blivet-3.9.1/COPYING.LESSER
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)  1301824 2024-02-27 09:43:00.000000 blivet-3.9.1/ChangeLog
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      160 2024-02-27 09:46:59.000000 blivet-3.9.1/MANIFEST.in
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6761 2024-02-27 09:46:59.000000 blivet-3.9.1/Makefile
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3872 2024-02-27 09:53:17.121024 blivet-3.9.1/PKG-INFO
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3285 2024-02-27 09:46:59.000000 blivet-3.9.1/README.md
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.108024 blivet-3.9.1/blivet/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4847 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13293 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/actionlist.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11283 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/arch.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    50365 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/blivet.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9454 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/callbacks.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.109023 blivet-3.9.1/blivet/dbus/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1014 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1982 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/action.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10041 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/blivet.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1732 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/constants.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3154 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/device.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2451 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/format.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2971 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/manager.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4749 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/dbus/object.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    43725 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/deviceaction.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    88252 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicefactory.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.109023 blivet-3.9.1/blivet/devicelibs/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1987 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/btrfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4838 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/crypto.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3521 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/disk.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32101 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/edd.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12465 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/gpt.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8795 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/lvm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1576 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/mdraid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    24513 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/raid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10243 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicelibs/stratis.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.110024 blivet-3.9.1/blivet/devices/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2063 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    27002 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/btrfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3726 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/cache.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7637 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/container.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13013 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/device.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25153 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/disk.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10783 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/dm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5288 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/file.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6614 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/lib.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4744 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/loop.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10130 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/luks.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   125598 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/lvm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    30768 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/md.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2087 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/network.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3032 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/nfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3743 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/nodev.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2849 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/optical.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    40429 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/partition.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4820 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/raid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32913 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/storage.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9857 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devices/stratis.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    42439 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/devicetree.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6730 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/errors.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.110024 blivet-3.9.1/blivet/events/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/events/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4285 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/events/changes.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11201 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/events/handler.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11428 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/events/manager.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8165 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/fcoe.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3897 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/flags.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.111024 blivet-3.9.1/blivet/formats/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25274 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2225 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/biosboot.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22796 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/disklabel.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2298 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/dmraid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    51778 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/fs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1699 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/fslib.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22591 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/luks.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9417 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/lvmpv.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3930 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/mdraid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2903 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/multipath.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3619 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/prepboot.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5200 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/stratis.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8750 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/formats/swap.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    30698 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/fstab.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2436 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/i18n.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    23264 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/iscsi.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6935 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/mounts.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3871 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/nvme.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    85044 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/partitioning.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.111024 blivet-3.9.1/blivet/populator/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/__init__.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.112023 blivet-3.9.1/blivet/populator/helpers/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2531 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2569 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/boot.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4453 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/btrfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2082 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/devicepopulator.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10895 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/disk.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6362 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/disklabel.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2524 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/dm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4241 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/formatpopulator.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2657 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/loop.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7445 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/luks.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    20156 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/lvm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9040 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/mdraid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2566 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/multipath.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2064 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/optical.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4284 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/partition.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2869 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/populatorhelper.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7591 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/helpers/stratis.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    21488 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/populator/populator.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8267 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/safe_dbus.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7154 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/size.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.112023 blivet-3.9.1/blivet/static_data/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      161 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/static_data/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3523 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/static_data/luks_data.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4047 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/static_data/lvm_info.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2431 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/static_data/mpath_info.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10260 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/static_data/stratis_info.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2687 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/storage_log.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.113024 blivet-3.9.1/blivet/tasks/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25914 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/availability.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1598 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/dfresize.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5413 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsck.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2652 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsinfo.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2789 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fslabeling.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5504 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsminsize.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11896 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsmkfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5945 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsmount.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2366 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsreadlabel.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3360 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsresize.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3079 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fssize.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2717 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fssync.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1784 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fstask.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2041 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fsuuid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2328 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fswritelabel.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1141 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/fswriteuuid.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3695 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/lukstasks.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2885 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/pvtask.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3333 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tasks/task.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3751 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/threads.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3459 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/tsort.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    34471 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/udev.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    36755 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/util.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    20888 2024-02-27 09:46:59.000000 blivet-3.9.1/blivet/zfcp.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.108024 blivet-3.9.1/blivet.egg-info/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3872 2024-02-27 09:53:17.000000 blivet-3.9.1/blivet.egg-info/PKG-INFO
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5213 2024-02-27 09:53:17.000000 blivet-3.9.1/blivet.egg-info/SOURCES.txt
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        1 2024-02-27 09:53:17.000000 blivet-3.9.1/blivet.egg-info/dependency_links.txt
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2024-02-27 09:53:17.000000 blivet-3.9.1/blivet.egg-info/requires.txt
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2024-02-27 09:53:17.000000 blivet-3.9.1/blivet.egg-info/top_level.txt
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.113024 blivet-3.9.1/dbus/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      400 2024-02-27 09:46:59.000000 blivet-3.9.1/dbus/blivet.conf
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      113 2024-02-27 09:46:59.000000 blivet-3.9.1/dbus/blivet.service
--rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)      364 2024-02-27 09:46:59.000000 blivet-3.9.1/dbus/blivetd
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      106 2024-02-27 09:46:59.000000 blivet-3.9.1/dbus/com.redhat.Blivet0.service
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.114024 blivet-3.9.1/examples/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/__init__.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2089 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/actions.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1071 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/btrfs.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      825 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/dbus_client.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1560 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/factory.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      205 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/list_devices.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2174 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1996 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm_cache.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1778 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm_cachepool.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2168 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm_non_linear.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1417 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm_thin.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2167 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/lvm_vdo.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2884 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/partitioning.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1816 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/stratis.py
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      526 2024-02-27 09:46:59.000000 blivet-3.9.1/examples/uevents.py
-drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:53:17.121024 blivet-3.9.1/po/
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1262 2024-02-27 09:42:12.000000 blivet-3.9.1/po/Makefile
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      944 2024-02-27 09:52:16.000000 blivet-3.9.1/po/af.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9722 2024-02-27 09:42:12.000000 blivet-3.9.1/po/af.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1059 2024-02-27 09:52:16.000000 blivet-3.9.1/po/am.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2024-02-27 09:42:12.000000 blivet-3.9.1/po/am.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1169 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ar.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10348 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ar.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9162 2024-02-27 09:52:16.000000 blivet-3.9.1/po/as.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15098 2024-02-27 09:42:12.000000 blivet-3.9.1/po/as.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3660 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ast.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11161 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ast.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8312 2024-02-27 09:52:16.000000 blivet-3.9.1/po/bg.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14404 2024-02-27 09:42:12.000000 blivet-3.9.1/po/bg.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9366 2024-02-27 09:42:12.000000 blivet-3.9.1/po/blivet.pot
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5487 2024-02-27 09:52:16.000000 blivet-3.9.1/po/bn.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13553 2024-02-27 09:42:12.000000 blivet-3.9.1/po/bn.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14554 2024-02-27 09:52:16.000000 blivet-3.9.1/po/bn_IN.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19308 2024-02-27 09:42:12.000000 blivet-3.9.1/po/bn_IN.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      939 2024-02-27 09:52:16.000000 blivet-3.9.1/po/bs.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9798 2024-02-27 09:42:12.000000 blivet-3.9.1/po/bs.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9908 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ca.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14680 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ca.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10656 2024-02-27 09:52:16.000000 blivet-3.9.1/po/cs.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14721 2024-02-27 09:42:12.000000 blivet-3.9.1/po/cs.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      943 2024-02-27 09:52:16.000000 blivet-3.9.1/po/cy.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9775 2024-02-27 09:42:12.000000 blivet-3.9.1/po/cy.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9554 2024-02-27 09:52:16.000000 blivet-3.9.1/po/da.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14077 2024-02-27 09:42:12.000000 blivet-3.9.1/po/da.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10456 2024-02-27 09:52:16.000000 blivet-3.9.1/po/de.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15434 2024-02-27 09:42:12.000000 blivet-3.9.1/po/de.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1239 2024-02-27 09:52:16.000000 blivet-3.9.1/po/de_CH.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10347 2024-02-27 09:42:12.000000 blivet-3.9.1/po/de_CH.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1377 2024-02-27 09:52:16.000000 blivet-3.9.1/po/el.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10406 2024-02-27 09:42:12.000000 blivet-3.9.1/po/el.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3591 2024-02-27 09:52:16.000000 blivet-3.9.1/po/en_GB.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11196 2024-02-27 09:42:12.000000 blivet-3.9.1/po/en_GB.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10416 2024-02-27 09:52:16.000000 blivet-3.9.1/po/es.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15603 2024-02-27 09:42:12.000000 blivet-3.9.1/po/es.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1280 2024-02-27 09:52:16.000000 blivet-3.9.1/po/et.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9997 2024-02-27 09:42:12.000000 blivet-3.9.1/po/et.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      620 2024-02-27 09:52:16.000000 blivet-3.9.1/po/eu.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9639 2024-02-27 09:42:12.000000 blivet-3.9.1/po/eu.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7338 2024-02-27 09:52:16.000000 blivet-3.9.1/po/fa.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13823 2024-02-27 09:42:12.000000 blivet-3.9.1/po/fa.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10323 2024-02-27 09:52:16.000000 blivet-3.9.1/po/fi.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14226 2024-02-27 09:42:12.000000 blivet-3.9.1/po/fi.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10981 2024-02-27 09:52:16.000000 blivet-3.9.1/po/fr.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15783 2024-02-27 09:42:12.000000 blivet-3.9.1/po/fr.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10674 2024-02-27 09:52:16.000000 blivet-3.9.1/po/fur.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14142 2024-02-27 09:42:12.000000 blivet-3.9.1/po/fur.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8423 2024-02-27 09:52:16.000000 blivet-3.9.1/po/gu.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14666 2024-02-27 09:42:12.000000 blivet-3.9.1/po/gu.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1655 2024-02-27 09:52:16.000000 blivet-3.9.1/po/he.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10117 2024-02-27 09:42:12.000000 blivet-3.9.1/po/he.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4840 2024-02-27 09:52:16.000000 blivet-3.9.1/po/hi.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12552 2024-02-27 09:42:12.000000 blivet-3.9.1/po/hi.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10464 2024-02-27 09:52:16.000000 blivet-3.9.1/po/hr.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14021 2024-02-27 09:42:12.000000 blivet-3.9.1/po/hr.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10051 2024-02-27 09:52:16.000000 blivet-3.9.1/po/hu.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15026 2024-02-27 09:42:12.000000 blivet-3.9.1/po/hu.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5160 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ia.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11904 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ia.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10366 2024-02-27 09:52:16.000000 blivet-3.9.1/po/id.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14243 2024-02-27 09:42:12.000000 blivet-3.9.1/po/id.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      945 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ilo.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ilo.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1053 2024-02-27 09:52:16.000000 blivet-3.9.1/po/is.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9763 2024-02-27 09:42:12.000000 blivet-3.9.1/po/is.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9517 2024-02-27 09:52:16.000000 blivet-3.9.1/po/it.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14933 2024-02-27 09:42:12.000000 blivet-3.9.1/po/it.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11782 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ja.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16274 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ja.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15844 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ka.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19403 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ka.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12917 2024-02-27 09:52:16.000000 blivet-3.9.1/po/kk.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16397 2024-02-27 09:42:12.000000 blivet-3.9.1/po/kk.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9449 2024-02-27 09:52:16.000000 blivet-3.9.1/po/kn.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15947 2024-02-27 09:42:12.000000 blivet-3.9.1/po/kn.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10951 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ko.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14945 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ko.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1380 2024-02-27 09:52:16.000000 blivet-3.9.1/po/lv.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10006 2024-02-27 09:42:12.000000 blivet-3.9.1/po/lv.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1878 2024-02-27 09:52:16.000000 blivet-3.9.1/po/mai.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10481 2024-02-27 09:42:12.000000 blivet-3.9.1/po/mai.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      977 2024-02-27 09:52:16.000000 blivet-3.9.1/po/mk.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9971 2024-02-27 09:42:12.000000 blivet-3.9.1/po/mk.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8639 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ml.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15344 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ml.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8864 2024-02-27 09:52:16.000000 blivet-3.9.1/po/mr.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15305 2024-02-27 09:42:12.000000 blivet-3.9.1/po/mr.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      890 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ms.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9755 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ms.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9565 2024-02-27 09:52:16.000000 blivet-3.9.1/po/nb.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13988 2024-02-27 09:42:12.000000 blivet-3.9.1/po/nb.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1210 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ne.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10132 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ne.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10473 2024-02-27 09:52:16.000000 blivet-3.9.1/po/nl.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14532 2024-02-27 09:42:12.000000 blivet-3.9.1/po/nl.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      935 2024-02-27 09:52:16.000000 blivet-3.9.1/po/nso.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9713 2024-02-27 09:42:12.000000 blivet-3.9.1/po/nso.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8185 2024-02-27 09:52:16.000000 blivet-3.9.1/po/or.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14855 2024-02-27 09:42:12.000000 blivet-3.9.1/po/or.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9260 2024-02-27 09:52:16.000000 blivet-3.9.1/po/pa.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15365 2024-02-27 09:42:12.000000 blivet-3.9.1/po/pa.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10862 2024-02-27 09:52:16.000000 blivet-3.9.1/po/pl.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15246 2024-02-27 09:42:12.000000 blivet-3.9.1/po/pl.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10634 2024-02-27 09:52:16.000000 blivet-3.9.1/po/pt.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14452 2024-02-27 09:42:12.000000 blivet-3.9.1/po/pt.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10764 2024-02-27 09:52:16.000000 blivet-3.9.1/po/pt_BR.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15596 2024-02-27 09:42:12.000000 blivet-3.9.1/po/pt_BR.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      951 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ro.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ro.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13409 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ru.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18138 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ru.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4859 2024-02-27 09:52:16.000000 blivet-3.9.1/po/si.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12466 2024-02-27 09:42:12.000000 blivet-3.9.1/po/si.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10698 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sk.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14702 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sk.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      953 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sl.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9987 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sl.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1052 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sq.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9767 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sq.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9864 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sr.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15052 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sr.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3409 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sr@latin.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11051 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sr@latin.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10387 2024-02-27 09:52:16.000000 blivet-3.9.1/po/sv.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14443 2024-02-27 09:42:12.000000 blivet-3.9.1/po/sv.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8111 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ta.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15091 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ta.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9153 2024-02-27 09:52:16.000000 blivet-3.9.1/po/te.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15384 2024-02-27 09:42:12.000000 blivet-3.9.1/po/te.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      769 2024-02-27 09:52:16.000000 blivet-3.9.1/po/tg.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9652 2024-02-27 09:42:12.000000 blivet-3.9.1/po/tg.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1471 2024-02-27 09:52:16.000000 blivet-3.9.1/po/th.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10233 2024-02-27 09:42:12.000000 blivet-3.9.1/po/th.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10625 2024-02-27 09:52:16.000000 blivet-3.9.1/po/tr.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14535 2024-02-27 09:42:12.000000 blivet-3.9.1/po/tr.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13478 2024-02-27 09:52:16.000000 blivet-3.9.1/po/uk.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    17502 2024-02-27 09:42:12.000000 blivet-3.9.1/po/uk.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      987 2024-02-27 09:52:16.000000 blivet-3.9.1/po/ur.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9759 2024-02-27 09:42:12.000000 blivet-3.9.1/po/ur.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2024-02-27 09:52:16.000000 blivet-3.9.1/po/zh_CN.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13838 2024-02-27 09:42:12.000000 blivet-3.9.1/po/zh_CN.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8734 2024-02-27 09:52:16.000000 blivet-3.9.1/po/zh_TW.mo
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13649 2024-02-27 09:42:12.000000 blivet-3.9.1/po/zh_TW.po
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   208679 2024-02-27 09:46:59.000000 blivet-3.9.1/python-blivet.spec
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16344 2024-02-27 09:46:59.000000 blivet-3.9.1/release_notes.rst
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2024-02-27 09:53:17.121024 blivet-3.9.1/setup.cfg
--rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3553 2024-02-27 09:46:59.000000 blivet-3.9.1/setup.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.407891 blivet-3.9.2/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18092 2024-02-27 09:46:59.000000 blivet-3.9.2/COPYING
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26530 2024-02-27 09:46:59.000000 blivet-3.9.2/COPYING.LESSER
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)  1309975 2024-03-28 12:13:24.000000 blivet-3.9.2/ChangeLog
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      160 2024-02-27 09:46:59.000000 blivet-3.9.2/MANIFEST.in
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6761 2024-03-07 08:41:42.000000 blivet-3.9.2/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3872 2024-03-28 12:15:41.406890 blivet-3.9.2/PKG-INFO
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3285 2024-03-07 08:41:42.000000 blivet-3.9.2/README.md
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.393890 blivet-3.9.2/blivet/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4847 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13286 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/actionlist.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11283 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/arch.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    50743 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/blivet.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9454 2024-03-06 12:20:06.000000 blivet-3.9.2/blivet/callbacks.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.394890 blivet-3.9.2/blivet/dbus/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1014 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1982 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/action.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10041 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/dbus/blivet.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1732 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/constants.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3154 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/device.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2451 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/format.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2971 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/dbus/manager.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4749 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/dbus/object.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    43725 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/deviceaction.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    88252 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devicefactory.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.394890 blivet-3.9.2/blivet/devicelibs/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devicelibs/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2147 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/devicelibs/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4838 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devicelibs/crypto.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3521 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devicelibs/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32101 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devicelibs/edd.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12465 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devicelibs/gpt.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8795 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devicelibs/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1576 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devicelibs/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    24513 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devicelibs/raid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10243 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devicelibs/stratis.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.395891 blivet-3.9.2/blivet/devices/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2063 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    27323 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/devices/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3726 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/cache.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7637 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/container.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13013 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/device.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25153 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devices/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10783 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devices/dm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5288 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devices/file.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6614 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devices/lib.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4744 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devices/loop.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10130 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   125598 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    30768 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/md.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2087 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devices/network.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3032 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devices/nfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3743 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devices/nodev.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2849 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/devices/optical.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    40845 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/devices/partition.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4820 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devices/raid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32913 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/devices/storage.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9936 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/devices/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    42439 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/devicetree.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6730 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/errors.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.395891 blivet-3.9.2/blivet/events/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/events/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4285 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/events/changes.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11201 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/events/handler.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11428 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/events/manager.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8165 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/fcoe.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3897 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/flags.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.396890 blivet-3.9.2/blivet/formats/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25274 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/formats/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2225 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/formats/biosboot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22796 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/disklabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2298 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/dmraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    52298 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/formats/fs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1699 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/formats/fslib.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22591 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/formats/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9417 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/lvmpv.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3930 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2903 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/formats/multipath.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3619 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/formats/prepboot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5200 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8750 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/formats/swap.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32334 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/fstab.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2436 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/i18n.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    23264 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/iscsi.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6935 2024-03-06 12:20:13.000000 blivet-3.9.2/blivet/mounts.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3871 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/nvme.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    85044 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/partitioning.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.396890 blivet-3.9.2/blivet/populator/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/__init__.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.397890 blivet-3.9.2/blivet/populator/helpers/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2531 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/helpers/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2569 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/populator/helpers/boot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4453 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2082 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/devicepopulator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10895 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/populator/helpers/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6362 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/helpers/disklabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2524 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/helpers/dm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4241 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/formatpopulator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2657 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/populator/helpers/loop.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7445 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/helpers/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    20156 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/populator/helpers/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9040 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/populator/helpers/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2566 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/multipath.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2064 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/optical.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4284 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/helpers/partition.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2869 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/populatorhelper.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7591 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/populator/helpers/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    21488 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/populator/populator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8267 2024-03-06 12:20:13.000000 blivet-3.9.2/blivet/safe_dbus.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7154 2024-03-06 12:20:13.000000 blivet-3.9.2/blivet/size.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.397890 blivet-3.9.2/blivet/static_data/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      161 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/static_data/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3523 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/static_data/luks_data.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4047 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/static_data/lvm_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2431 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/static_data/mpath_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10260 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/static_data/stratis_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2687 2024-03-06 12:20:13.000000 blivet-3.9.2/blivet/storage_log.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.398891 blivet-3.9.2/blivet/tasks/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-06 12:19:40.000000 blivet-3.9.2/blivet/tasks/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26251 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/tasks/availability.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1598 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/dfresize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5413 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsck.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2652 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsinfo.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2789 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fslabeling.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5504 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsminsize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11896 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsmkfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5945 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/fsmount.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2366 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsreadlabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3360 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/fsresize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3079 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fssize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2717 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fssync.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1784 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fstask.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2041 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/fsuuid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2328 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/fswritelabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1141 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/fswriteuuid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3695 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/lukstasks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2885 2024-03-07 08:41:42.000000 blivet-3.9.2/blivet/tasks/pvtask.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3333 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/tasks/task.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3751 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/threads.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3459 2024-03-06 12:20:13.000000 blivet-3.9.2/blivet/tsort.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    34471 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/udev.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    36765 2024-03-28 12:15:11.000000 blivet-3.9.2/blivet/util.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    20888 2024-03-28 12:04:56.000000 blivet-3.9.2/blivet/zfcp.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.393890 blivet-3.9.2/blivet.egg-info/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3872 2024-03-28 12:15:41.000000 blivet-3.9.2/blivet.egg-info/PKG-INFO
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5213 2024-03-28 12:15:41.000000 blivet-3.9.2/blivet.egg-info/SOURCES.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        1 2024-03-28 12:15:41.000000 blivet-3.9.2/blivet.egg-info/dependency_links.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2024-03-28 12:15:41.000000 blivet-3.9.2/blivet.egg-info/requires.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2024-03-28 12:15:41.000000 blivet-3.9.2/blivet.egg-info/top_level.txt
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.398891 blivet-3.9.2/dbus/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      400 2024-02-27 09:46:59.000000 blivet-3.9.2/dbus/blivet.conf
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      113 2024-02-27 09:46:59.000000 blivet-3.9.2/dbus/blivet.service
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)      364 2024-02-27 09:46:59.000000 blivet-3.9.2/dbus/blivetd
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      106 2024-02-27 09:46:59.000000 blivet-3.9.2/dbus/com.redhat.Blivet0.service
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.399891 blivet-3.9.2/examples/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2089 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/actions.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1071 2024-03-07 08:41:42.000000 blivet-3.9.2/examples/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      825 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/dbus_client.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1560 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/factory.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      205 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/list_devices.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2174 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1996 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm_cache.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1778 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm_cachepool.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2168 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm_non_linear.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1417 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm_thin.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2167 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/lvm_vdo.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2884 2024-03-07 08:41:42.000000 blivet-3.9.2/examples/partitioning.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1816 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      526 2024-02-27 09:46:59.000000 blivet-3.9.2/examples/uevents.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2024-03-28 12:15:41.406890 blivet-3.9.2/po/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1262 2024-03-28 12:07:32.000000 blivet-3.9.2/po/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      944 2024-03-28 12:15:41.000000 blivet-3.9.2/po/af.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9722 2024-03-28 12:07:32.000000 blivet-3.9.2/po/af.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1059 2024-03-28 12:15:41.000000 blivet-3.9.2/po/am.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2024-03-28 12:07:32.000000 blivet-3.9.2/po/am.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1169 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ar.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10348 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ar.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9162 2024-03-28 12:15:41.000000 blivet-3.9.2/po/as.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15098 2024-03-28 12:07:32.000000 blivet-3.9.2/po/as.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3660 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ast.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11161 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ast.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8312 2024-03-28 12:15:41.000000 blivet-3.9.2/po/bg.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14404 2024-03-28 12:07:32.000000 blivet-3.9.2/po/bg.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9366 2024-03-28 12:07:32.000000 blivet-3.9.2/po/blivet.pot
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5487 2024-03-28 12:15:41.000000 blivet-3.9.2/po/bn.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13553 2024-03-28 12:07:32.000000 blivet-3.9.2/po/bn.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14554 2024-03-28 12:15:41.000000 blivet-3.9.2/po/bn_IN.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19308 2024-03-28 12:07:32.000000 blivet-3.9.2/po/bn_IN.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      939 2024-03-28 12:15:41.000000 blivet-3.9.2/po/bs.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9798 2024-03-28 12:07:32.000000 blivet-3.9.2/po/bs.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9908 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ca.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14680 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ca.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10656 2024-03-28 12:15:41.000000 blivet-3.9.2/po/cs.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14721 2024-03-28 12:07:32.000000 blivet-3.9.2/po/cs.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      943 2024-03-28 12:15:41.000000 blivet-3.9.2/po/cy.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9775 2024-03-28 12:07:32.000000 blivet-3.9.2/po/cy.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9554 2024-03-28 12:15:41.000000 blivet-3.9.2/po/da.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14077 2024-03-28 12:07:32.000000 blivet-3.9.2/po/da.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10456 2024-03-28 12:15:41.000000 blivet-3.9.2/po/de.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15434 2024-03-28 12:07:32.000000 blivet-3.9.2/po/de.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1239 2024-03-28 12:15:41.000000 blivet-3.9.2/po/de_CH.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10347 2024-03-28 12:07:32.000000 blivet-3.9.2/po/de_CH.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1377 2024-03-28 12:15:41.000000 blivet-3.9.2/po/el.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10406 2024-03-28 12:07:32.000000 blivet-3.9.2/po/el.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3591 2024-03-28 12:15:41.000000 blivet-3.9.2/po/en_GB.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11196 2024-03-28 12:07:32.000000 blivet-3.9.2/po/en_GB.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10416 2024-03-28 12:15:41.000000 blivet-3.9.2/po/es.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15603 2024-03-28 12:07:32.000000 blivet-3.9.2/po/es.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1280 2024-03-28 12:15:41.000000 blivet-3.9.2/po/et.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9997 2024-03-28 12:07:32.000000 blivet-3.9.2/po/et.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      620 2024-03-28 12:15:41.000000 blivet-3.9.2/po/eu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9639 2024-03-28 12:07:32.000000 blivet-3.9.2/po/eu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7338 2024-03-28 12:15:41.000000 blivet-3.9.2/po/fa.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13823 2024-03-28 12:07:32.000000 blivet-3.9.2/po/fa.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10323 2024-03-28 12:15:41.000000 blivet-3.9.2/po/fi.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14226 2024-03-28 12:07:32.000000 blivet-3.9.2/po/fi.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10981 2024-03-28 12:15:41.000000 blivet-3.9.2/po/fr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15783 2024-03-28 12:07:32.000000 blivet-3.9.2/po/fr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10674 2024-03-28 12:15:41.000000 blivet-3.9.2/po/fur.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14142 2024-03-28 12:07:32.000000 blivet-3.9.2/po/fur.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8423 2024-03-28 12:15:41.000000 blivet-3.9.2/po/gu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14666 2024-03-28 12:07:32.000000 blivet-3.9.2/po/gu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1655 2024-03-28 12:15:41.000000 blivet-3.9.2/po/he.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10117 2024-03-28 12:07:32.000000 blivet-3.9.2/po/he.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4840 2024-03-28 12:15:41.000000 blivet-3.9.2/po/hi.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12552 2024-03-28 12:07:32.000000 blivet-3.9.2/po/hi.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10464 2024-03-28 12:15:41.000000 blivet-3.9.2/po/hr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14021 2024-03-28 12:07:32.000000 blivet-3.9.2/po/hr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10051 2024-03-28 12:15:41.000000 blivet-3.9.2/po/hu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15026 2024-03-28 12:07:32.000000 blivet-3.9.2/po/hu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5160 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ia.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11904 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ia.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10366 2024-03-28 12:15:41.000000 blivet-3.9.2/po/id.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14243 2024-03-28 12:07:32.000000 blivet-3.9.2/po/id.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      945 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ilo.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ilo.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1053 2024-03-28 12:15:41.000000 blivet-3.9.2/po/is.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9763 2024-03-28 12:07:32.000000 blivet-3.9.2/po/is.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9517 2024-03-28 12:15:41.000000 blivet-3.9.2/po/it.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14933 2024-03-28 12:07:32.000000 blivet-3.9.2/po/it.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11782 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ja.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16274 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ja.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15844 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ka.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19403 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ka.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12917 2024-03-28 12:15:41.000000 blivet-3.9.2/po/kk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16397 2024-03-28 12:07:32.000000 blivet-3.9.2/po/kk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9449 2024-03-28 12:15:41.000000 blivet-3.9.2/po/kn.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15947 2024-03-28 12:07:32.000000 blivet-3.9.2/po/kn.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10951 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ko.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14945 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ko.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1380 2024-03-28 12:15:41.000000 blivet-3.9.2/po/lv.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10006 2024-03-28 12:07:32.000000 blivet-3.9.2/po/lv.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1878 2024-03-28 12:15:41.000000 blivet-3.9.2/po/mai.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10481 2024-03-28 12:07:32.000000 blivet-3.9.2/po/mai.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      977 2024-03-28 12:15:41.000000 blivet-3.9.2/po/mk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9971 2024-03-28 12:07:32.000000 blivet-3.9.2/po/mk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8639 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ml.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15344 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ml.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8864 2024-03-28 12:15:41.000000 blivet-3.9.2/po/mr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15305 2024-03-28 12:07:32.000000 blivet-3.9.2/po/mr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      890 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ms.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9755 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ms.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9565 2024-03-28 12:15:41.000000 blivet-3.9.2/po/nb.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13988 2024-03-28 12:07:32.000000 blivet-3.9.2/po/nb.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1210 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ne.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10132 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ne.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10473 2024-03-28 12:15:41.000000 blivet-3.9.2/po/nl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14532 2024-03-28 12:07:32.000000 blivet-3.9.2/po/nl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      935 2024-03-28 12:15:41.000000 blivet-3.9.2/po/nso.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9713 2024-03-28 12:07:32.000000 blivet-3.9.2/po/nso.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8185 2024-03-28 12:15:41.000000 blivet-3.9.2/po/or.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14855 2024-03-28 12:07:32.000000 blivet-3.9.2/po/or.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9260 2024-03-28 12:15:41.000000 blivet-3.9.2/po/pa.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15365 2024-03-28 12:07:32.000000 blivet-3.9.2/po/pa.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10862 2024-03-28 12:15:41.000000 blivet-3.9.2/po/pl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15246 2024-03-28 12:07:32.000000 blivet-3.9.2/po/pl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10634 2024-03-28 12:15:41.000000 blivet-3.9.2/po/pt.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14452 2024-03-28 12:07:32.000000 blivet-3.9.2/po/pt.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10764 2024-03-28 12:15:41.000000 blivet-3.9.2/po/pt_BR.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15596 2024-03-28 12:07:32.000000 blivet-3.9.2/po/pt_BR.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      951 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ro.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ro.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13409 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ru.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18138 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ru.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4859 2024-03-28 12:15:41.000000 blivet-3.9.2/po/si.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12466 2024-03-28 12:07:32.000000 blivet-3.9.2/po/si.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10698 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14702 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      953 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9987 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1052 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sq.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9767 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sq.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9864 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15052 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3409 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sr@latin.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11051 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sr@latin.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10387 2024-03-28 12:15:41.000000 blivet-3.9.2/po/sv.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14443 2024-03-28 12:07:32.000000 blivet-3.9.2/po/sv.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8111 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ta.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15091 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ta.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9153 2024-03-28 12:15:41.000000 blivet-3.9.2/po/te.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15384 2024-03-28 12:07:32.000000 blivet-3.9.2/po/te.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      769 2024-03-28 12:15:41.000000 blivet-3.9.2/po/tg.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9652 2024-03-28 12:07:32.000000 blivet-3.9.2/po/tg.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1471 2024-03-28 12:15:41.000000 blivet-3.9.2/po/th.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10233 2024-03-28 12:07:32.000000 blivet-3.9.2/po/th.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10625 2024-03-28 12:15:41.000000 blivet-3.9.2/po/tr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14535 2024-03-28 12:07:32.000000 blivet-3.9.2/po/tr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13478 2024-03-28 12:15:41.000000 blivet-3.9.2/po/uk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    17502 2024-03-28 12:07:32.000000 blivet-3.9.2/po/uk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      987 2024-03-28 12:15:41.000000 blivet-3.9.2/po/ur.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9759 2024-03-28 12:07:32.000000 blivet-3.9.2/po/ur.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2024-03-28 12:15:41.000000 blivet-3.9.2/po/zh_CN.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13838 2024-03-28 12:07:32.000000 blivet-3.9.2/po/zh_CN.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8734 2024-03-28 12:15:41.000000 blivet-3.9.2/po/zh_TW.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13649 2024-03-28 12:07:32.000000 blivet-3.9.2/po/zh_TW.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   209700 2024-03-28 12:15:11.000000 blivet-3.9.2/python-blivet.spec
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16344 2024-03-28 12:04:56.000000 blivet-3.9.2/release_notes.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2024-03-28 12:15:41.407891 blivet-3.9.2/setup.cfg
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3553 2024-03-28 12:15:11.000000 blivet-3.9.2/setup.py
```

### Comparing `blivet-3.9.1/COPYING` & `blivet-3.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/COPYING.LESSER` & `blivet-3.9.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/ChangeLog` & `blivet-3.9.2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,249 @@
+commit 0fbc1d43e0931802eb952de038756c2e2ed28021
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 28 13:13:07 2024 +0100
+
+    New version: 3.9.2
+
+commit c69120059544eb6d4eada3d891d49db06490d20c
+Merge: e5dd270a 39931945
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 28 13:07:19 2024 +0100
+
+    Merge remote-tracking branch 'origin/3.9-devel' into 3.9-release
+
+commit 39931945a355c2e61bd6c6a99124de5864978166
+Merge: 69faaf30 edb23194
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 28 12:24:19 2024 +0100
+
+    Merge pull request #1217 from vojtechtrefny/3.9-devel_btrfs-list-subvolumes-fix
+    
+    Misc fixes related to btrfs subvolume listing
+
+commit edb231949908a4e89b3321646f5b1c7276265bf0
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 27 13:50:59 2024 +0100
+
+    tests: Add a simple unit test for listing btrfs subvolumes
+
+commit 2698bad1211a666a67c30a11873e75cd0a6ce7f1
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 27 13:33:58 2024 +0100
+
+    Fix getting default subvolume ID for mounted btrfs volumes
+    
+    We already have the mountpoint from the previous list subvolumes
+    operations so we can just use it here too.
+
+commit 012d28c1523c9fca0d3452a67f505f6225da1347
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 27 13:32:41 2024 +0100
+
+    Do not try to get btrfs subvolumes without libblockdev
+    
+    We have the libblockdev call in try-except but it still creates an
+    unnecessary call and mount operation for something that must fail
+    when the plugin is not loaded.
+
+commit 69faaf3068835c44bdadc12feca81e78c961e69c
+Merge: f25199d4 038799f7
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 27 08:10:32 2024 +0100
+
+    Merge pull request #1216 from vojtechtrefny/3.9-devel_btrfs-is-empty-subvolumes-fix
+    
+    Do not raise not implemented exception when checking if btrfs is empty
+
+commit 038799f79b9d4cd5184a4a8367b3e3963aa7ed2f
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Tue Mar 26 13:51:48 2024 +0100
+
+    Do not raise not implemented exception when checking if btrfs is empty
+    
+    If we don't have libblockdev btrfs plugin we cannot check if the
+    btrfs filesystem is empty.
+
+commit f25199d491956fd908eaecdee45f5174d192b5e6
+Merge: fa0c6853 2a8f0028
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 20 13:58:31 2024 +0100
+
+    Merge pull request #1210 from vojtechtrefny/3.9-devel_type-uuid-print-fix
+    
+    Fix printing the partition type UUID
+
+commit fa0c68531467be088fc8f6a8a8d79cdfcfbce112
+Merge: 66914f0e 4e2c9e89
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 20 13:58:14 2024 +0100
+
+    Merge pull request #1213 from vojtechtrefny/3.9-devel_stratis-service-start
+    
+    Try to start stratisd before checking its availability
+
+commit 66914f0ee20bd6af61835547b1ce3ee3dd24833e
+Merge: dcee26b0 4680e447
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Tue Mar 19 13:24:07 2024 +0100
+
+    Merge pull request #1212 from vojtechtrefny/3.9-devel_stratis-no-size-fix
+    
+    Fix creating Stratis filesystem without size specified
+
+commit 4e2c9e89bdb41688786a50244d40a3dd71f8ce10
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Tue Mar 19 13:20:31 2024 +0100
+
+    Try to start stratisd before checking its availability
+    
+    stratisd is neither autostarted after installing the package nor
+    DBus activated so we need to try to start it first.
+
+commit 4680e44709b328c7f75004b26670ebf431c6b161
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 18 14:35:04 2024 +0100
+
+    Fix creating Stratis filesystem without size specified
+    
+    We do allow creating Stratis FS without specifying its size which
+    simply means creating the default 1 TiB filesystem.
+
+commit 2a8f0028420233d6efc4307a30a0df14538b2116
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 14 09:37:49 2024 +0100
+
+    Fix printing the partition type UUID
+    
+    We want to print the human-readable string if possible, not the
+    binary data.
+
+commit dcee26b0a84546aa7db93272101d55e6346884e7
+Merge: 7fa3d195 f70c8fc6
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Tue Mar 12 10:27:20 2024 +0100
+
+    Merge pull request #1208 from vojtechtrefny/3.9-devel_fix-btrfs-is-empty
+    
+    Adjust check for btrfs filesystem being empty
+
+commit f70c8fc68db656171a92ccc83b201837ed1e5aa7
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 11 14:42:46 2024 +0100
+
+    Adjust check for btrfs filesystem being empty
+    
+    There are some changes planned in libblockdev that will affect how
+    subvolumes are listed so we need to adjust our check to work with
+    both the old and new version of libblockdev.
+
+commit 7fa3d195c644396c3fabacc0c6ea38074f00d24c
+Merge: 9d9cd86d dca4de17
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 7 13:13:06 2024 +0100
+
+    Merge pull request #1204 from vojtechtrefny/3.9-devel_missing-fstab
+    
+    Fixes for latest Ubuntu/Debian support
+
+commit 9d9cd86d70edb5ab4538de6eeddb9e7fc6eebe5f
+Merge: 8341d80b 2917d8f9
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 7 10:06:11 2024 +0100
+
+    Merge pull request #1207 from vojtechtrefny/3.9-devel_detect-virt-amazon
+    
+    Fix util.detect_virt on Amazon
+
+commit 2917d8f99978206b3d1fbf9842ae708db02dfbd3
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Thu Mar 7 09:45:28 2024 +0100
+
+    Fix util.detect_virt on Amazon
+
+commit dca4de17e39f3032cfeb658dcdc7eebc5e30469f
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 4 15:34:38 2024 +0100
+
+    misc: Vagrantfile update
+
+commit 55e0893ab296863449a6f9ca687e38ea6dabec27
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 4 15:09:39 2024 +0100
+
+    misc: Run pip with --break-system-packages
+    
+    We are installing packages using pip system-wide so we need to add
+    --break-system-packages to make it work.
+
+commit ddcc0be893c0064126579d0fa5979d57c5ddfb4b
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 4 15:09:10 2024 +0100
+
+    misc: Add missing libmount build dependencies
+
+commit 8c2c1559b71bfe2d3f7657f1483afcc8aced005f
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 4 15:08:00 2024 +0100
+
+    availability: Check for mpath friendly names availability
+    
+    We set the friendly names feature during populate so we need to
+    check for its support (which requires mpathconf) too.
+
+commit ab90f792462bd2a3410ab528fd5452054e1fb656
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Mon Mar 4 15:07:02 2024 +0100
+
+    Allow running blivet without libmount Python bindings
+    
+    The libmount bindings are not available everywhere so we should
+    make sure blivet still can be used without it if fstab management
+    is not required.
+
+commit 8341d80bb4313725e764820cd51b826bfa12f009
+Merge: e0b33c92 ef65defc
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 6 15:30:09 2024 +0100
+
+    Merge pull request #1197 from japokorn/3.9-devel-fstab_cleanup_fix
+    
+    Fstab cleanup fix
+
+commit e0b33c923d47ca646d9dff0b209994c86a93dc5a
+Merge: 94adfec2 afa91842
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Wed Mar 6 15:29:25 2024 +0100
+
+    Merge pull request #1205 from vojtechtrefny/3.9-devel_fix-btrfs-mountpoint-check
+    
+    Fix getting subvolumes for mounted btrfs volumes
+
+commit ef65defc14e3cfc849bad2110339deb7924d4b64
+Author: Jan Pokorny <japokorn@redhat.com>
+Date:   Thu Feb 8 15:13:02 2024 +0100
+
+    Fstab cleanup fix
+    
+    Formats with multiple layers (e.g. LUKS) were not handled properly in
+    fstab. This resulted in fstab entries not being properly cleaned from
+    fstab when destroy actions were executed. This fixes the issue by using
+    different variables with correct values based on action type.
+
+commit afa91842ff01982823d891d57650a387fd69ad31
+Author: Vojtech Trefny <vtrefny@redhat.com>
+Date:   Tue Mar 5 14:42:23 2024 +0100
+
+    Fix getting subvolumes for mounted btrfs volumes
+    
+    When looking for a mountpoint we're trying to compare device name
+    with the device node base name which doesn't work for DM devices
+    like LUKS (we're trying to compare "dm-0" to "luks-..."), we need
+    to make sure to resolve the name first.
+
 commit e5dd270af952460007ed0b517a489849179d45f4
 Author: Vojtech Trefny <vtrefny@redhat.com>
 Date:   Tue Feb 27 10:42:46 2024 +0100
 
     New version: 3.9.1
 
 commit c8fa34f30cea83d61d90203b47e6fdc78214cd17
```

### Comparing `blivet-3.9.1/Makefile` & `blivet-3.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/PKG-INFO` & `blivet-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blivet
-Version: 3.9.1
+Version: 3.9.2
 Summary: Python module for system storage configuration
 Home-page: http://github.com/storaged-project/blivet
 Author: David Lehman
 Author-email: dlehman@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `blivet-3.9.1/README.md` & `blivet-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/__init__.py` & `blivet-3.9.2/blivet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #                    Vratislav Podzimek <vpodzime@redhat.com>
 #
 
-__version__ = '3.9.1'
+__version__ = '3.9.2'
 
 import sys
 import importlib
 import warnings
 import syslog
 
 from . import arch
```

### Comparing `blivet-3.9.1/blivet/actionlist.py` & `blivet-3.9.2/blivet/actionlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
             if dry_run:
                 continue
 
             # get (b)efore (a)ction.(e)xecute fstab entry
             # (device may not exist afterwards)
             if not skip_fstab:
                 try:
-                    entry = fstab.entry_from_device(action.device)
+                    entry = fstab.entry_from_action(action)
                 except ValueError:
                     # this device should not be in fstab
                     bae_entry = None
                 else:
                     bae_entry = fstab.find_entry(entry=entry)
 
             with blivet_lock:
```

### Comparing `blivet-3.9.1/blivet/arch.py` & `blivet-3.9.2/blivet/arch.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/blivet.py` & `blivet-3.9.2/blivet/blivet.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from .deviceaction import ActionDestroyFormat, ActionResizeDevice, ActionResizeFormat
 from .devicelibs.edd import get_edd_dict
 from .devicelibs.btrfs import MAIN_VOLUME_ID
 from .devicelibs.crypto import LUKS_METADATA_SIZE
 from .errors import StorageError, DependencyError
 from .size import Size
 from .devicetree import DeviceTree
-from .fstab import FSTabManager
+from .fstab import FSTabManager, HAVE_LIBMOUNT
 from .formats import get_default_filesystem_type
 from .flags import flags
 from .formats import get_format
 from .util import capture_output, natural_sort_key
 from . import arch
 from . import devicefactory
 from . import __version__
@@ -52,15 +52,18 @@
 from .threads import SynchronizedMeta
 from .static_data import luks_data
 
 import logging
 log = logging.getLogger("blivet")
 
 
-FSTAB_PATH = "/etc/fstab"
+# Default path to fstab file. Left empty to prevent blivet from using
+# fstab functionality by default.
+# TODO Change to "/etc/fstab" at next major version
+FSTAB_PATH = ""
 
 
 @six.add_metaclass(SynchronizedMeta)
 class Blivet(object):
 
     """ Top-level class for managing storage configuration. """
 
@@ -71,17 +74,21 @@
         self.ignored_disks = []
         self.exclusive_disks = []
         self.disk_images = {}
 
         self.size_sets = []
         self.set_default_fstype(get_default_filesystem_type())
 
-        # fstab write location purposedly set to None. It has to be overriden
+        # fstab write location purposedly set to None. It has to be overridden
         # manually when using blivet.
-        self.fstab = FSTabManager(src_file=FSTAB_PATH, dest_file=None)
+        if HAVE_LIBMOUNT:
+            self.fstab = FSTabManager(src_file=FSTAB_PATH, dest_file=None)
+        else:
+            log.info("Python libmount bindings missing, fstab management is disabled")
+            self.fstab = None
 
         self._short_product_name = 'blivet'
 
         self._next_id = 0
         self._dump_file = "%s/storage.state" % tempfile.gettempdir()
 
         try:
@@ -116,15 +123,17 @@
 
         :param callbacks: callbacks to be invoked when actions are executed
         :type callbacks: return value of the :func:`~.callbacks.create_new_callbacks_register`
 
         """
 
         self.devicetree.actions.process(callbacks=callbacks, devices=self.devices, fstab=self.fstab)
-        self.fstab.read()
+
+        if self.fstab:
+            self.fstab.read()
 
     @property
     def next_id(self):
         """ Used for creating unique placeholder names. """
         newid = self._next_id
         self._next_id += 1
         return newid
@@ -146,15 +155,16 @@
         self.devicetree.reset(ignored_disks=self.ignored_disks,
                               exclusive_disks=self.exclusive_disks,
                               disk_images=self.disk_images)
         self.devicetree.populate(cleanup_only=cleanup_only)
         self.edd_dict = get_edd_dict(self.partitioned)
         self.devicetree.edd_dict = self.edd_dict
 
-        self.fstab.read()
+        if self.fstab:
+            self.fstab.read()
 
         if flags.include_nodev:
             self.devicetree.handle_nodev_filesystems()
 
     @property
     def devices(self):
         """ A list of all the devices in the device tree. """
```

### Comparing `blivet-3.9.1/blivet/callbacks.py` & `blivet-3.9.2/blivet/callbacks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/__init__.py` & `blivet-3.9.2/blivet/dbus/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/action.py` & `blivet-3.9.2/blivet/dbus/action.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/blivet.py` & `blivet-3.9.2/blivet/dbus/blivet.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/constants.py` & `blivet-3.9.2/blivet/dbus/constants.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/device.py` & `blivet-3.9.2/blivet/dbus/device.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/format.py` & `blivet-3.9.2/blivet/dbus/format.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/manager.py` & `blivet-3.9.2/blivet/dbus/manager.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/dbus/object.py` & `blivet-3.9.2/blivet/dbus/object.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/deviceaction.py` & `blivet-3.9.2/blivet/deviceaction.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicefactory.py` & `blivet-3.9.2/blivet/devicefactory.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/btrfs.py` & `blivet-3.9.2/blivet/devicelibs/btrfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,9 +60,12 @@
     """
     if not os.path.ismount(mountpoint):
         raise ValueError("%s doesn't seem to be a mountpoint" % mountpoint)
     try:
         subvols = BlockDev.btrfs.list_subvolumes(mountpoint)
     except BlockDev.BtrfsError as e:
         raise BTRFSError(str(e))
+    except BlockDev.BlockDevNotImplementedError:
+        log.warning("cannot get list of subvolumes: libblockdev btrfs plugin not available")
+        return []
     else:
         return [s.path for s in subvols]
```

### Comparing `blivet-3.9.1/blivet/devicelibs/crypto.py` & `blivet-3.9.2/blivet/devicelibs/crypto.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/disk.py` & `blivet-3.9.2/blivet/devicelibs/disk.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/edd.py` & `blivet-3.9.2/blivet/devicelibs/edd.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/gpt.py` & `blivet-3.9.2/blivet/devicelibs/gpt.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/lvm.py` & `blivet-3.9.2/blivet/devicelibs/lvm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/mdraid.py` & `blivet-3.9.2/blivet/devicelibs/mdraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/raid.py` & `blivet-3.9.2/blivet/devicelibs/raid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devicelibs/stratis.py` & `blivet-3.9.2/blivet/devicelibs/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/__init__.py` & `blivet-3.9.2/blivet/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/btrfs.py` & `blivet-3.9.2/blivet/devices/btrfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ..flags import flags
 from ..storage_log import log_method_call
 from .. import udev
 from .. import util
 from ..formats import get_format, DeviceFormat
 from ..size import Size
 from ..mounts import mounts_cache
+from .. import missing_plugs
 
 import logging
 log = logging.getLogger("blivet")
 
 from .storage import StorageDevice
 from .container import ContainerDevice
 from .raid import RaidDevice
@@ -353,15 +354,15 @@
         if self.format.system_mountpoint:
             return self.format.system_mountpoint
         if self.original_format.system_mountpoint:
             return self.original_format.system_mountpoint
 
         # now try every possible mountpoint with any subvolspec in our cache
         parents = [p.name for p in self.parents]
-        mount_spec = next(((dev, subvol) for dev, subvol in mounts_cache.mountpoints if dev in parents), None)
+        mount_spec = next(((dev, subvol) for dev, subvol in mounts_cache.mountpoints if udev.resolve_devspec(dev) in parents), None)
         if mount_spec:
             try:
                 return mounts_cache.get_mountpoints(devspec=mount_spec[0],
                                                     subvolspec=mount_spec[1])[-1]
             except IndexError:
                 return None
         return None
@@ -370,20 +371,25 @@
         subvols = []
         try:
             subvols = blockdev.btrfs.list_subvolumes(mountpoint,
                                                      snapshots_only=snapshots_only)
         except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as e:
             log.debug("failed to list subvolumes: %s", e)
         else:
-            self._get_default_subvolume_id()
+            self._get_default_subvolume_id(mountpoint)
 
         return subvols
 
     def list_subvolumes(self, snapshots_only=False):
         subvols = []
+
+        if "btrfs" in missing_plugs:
+            log.debug("not listing btrfs subvolumes, libblockdev btrfs plugin is missing")
+            return subvols
+
         if flags.auto_dev_updates:
             self.setup(orig=True)
 
         # for list_subvolumes we can use mountpoint of a subvolume too, the volume
         # itself doesn't need to be mounted
         mountpoint = self._get_any_btrfs_mountpoint()
         if mountpoint:
@@ -400,21 +406,24 @@
                 pass
 
         return subvols
 
     def remove_subvolume(self, name):
         raise NotImplementedError()
 
-    def _get_default_subvolume_id(self):
+    def _get_default_subvolume_id(self, mountpoint=None):
         subvolid = None
-        with self._do_temp_mount() as mountpoint:
-            try:
+
+        try:
+            if mountpoint:
+                subvolid = blockdev.btrfs.get_default_subvolume_id(mountpoint)
+            elif flags.auto_dev_updates:
                 subvolid = blockdev.btrfs.get_default_subvolume_id(mountpoint)
-            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as e:
-                log.debug("failed to get default subvolume id: %s", e)
+        except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as e:
+            log.debug("failed to get default subvolume id: %s", e)
 
         self._default_subvolume_id = subvolid
 
     def _set_default_subvolume_id(self, vol_id):
         """ Set a new default subvolume by id.
 
             This writes the change to the filesystem, which must be mounted.
```

### Comparing `blivet-3.9.1/blivet/devices/cache.py` & `blivet-3.9.2/blivet/devices/cache.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/container.py` & `blivet-3.9.2/blivet/devices/container.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/device.py` & `blivet-3.9.2/blivet/devices/device.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/disk.py` & `blivet-3.9.2/blivet/devices/disk.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/dm.py` & `blivet-3.9.2/blivet/devices/dm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/file.py` & `blivet-3.9.2/blivet/devices/file.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/lib.py` & `blivet-3.9.2/blivet/devices/lib.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/loop.py` & `blivet-3.9.2/blivet/devices/loop.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/luks.py` & `blivet-3.9.2/blivet/devices/luks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/lvm.py` & `blivet-3.9.2/blivet/devices/lvm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/md.py` & `blivet-3.9.2/blivet/devices/md.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/network.py` & `blivet-3.9.2/blivet/devices/network.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/nfs.py` & `blivet-3.9.2/blivet/devices/nfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/nodev.py` & `blivet-3.9.2/blivet/devices/nodev.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/optical.py` & `blivet-3.9.2/blivet/devices/optical.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/partition.py` & `blivet-3.9.2/blivet/devices/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,16 +254,21 @@
         if self.parted_partition:
             s += ("  start = %(start)s  end = %(end)s  length = %(length)s\n"
                   "  flags = %(flags)s" %
                   {"length": self.parted_partition.geometry.length,
                    "start": self.parted_partition.geometry.start,
                    "end": self.parted_partition.geometry.end,
                    "flags": self.parted_partition.getFlagsAsString()})
-            if hasattr(parted.Partition, "type_uuid"):
-                s += " type_uuid = %s" % self.parted_partition.type_uuid
+            if hasattr(parted.Partition, "type_uuid") and self.parted_partition.type_uuid:
+                try:
+                    uuid_str = UUID(bytes=self.parted_partition.type_uuid)
+                except (TypeError, ValueError):
+                    pass
+                else:
+                    s += " type_uuid = %s" % uuid_str
         return s
 
     @property
     def dict(self):
         d = super(PartitionDevice, self).dict
         d.update({"type": self.part_type})
         if not self.exists:
@@ -272,16 +277,21 @@
                       "primary": self.req_primary})
 
         if self.parted_partition:
             d.update({"length": self.parted_partition.geometry.length,
                       "start": self.parted_partition.geometry.start,
                       "end": self.parted_partition.geometry.end,
                       "flags": self.parted_partition.getFlagsAsString()})
-            if hasattr(parted.Partition, "type_uuid"):
-                d.update({"type_uuid": self.parted_partition.type_uuid})
+            if hasattr(parted.Partition, "type_uuid") and self.parted_partition.type_uuid:
+                try:
+                    uuid_str = UUID(bytes=self.parted_partition.type_uuid)
+                except (TypeError, ValueError):
+                    pass
+                else:
+                    d.update({"type_uuid": uuid_str})
         return d
 
     def align_target_size(self, newsize):
         """ Return newsize adjusted to allow for an end-aligned partition.
 
             :param :class:`~.Size` newsize: proposed/unaligned target size
             :raises _ped.CreateException: if the size extends beyond the end of
```

### Comparing `blivet-3.9.1/blivet/devices/raid.py` & `blivet-3.9.2/blivet/devices/raid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/storage.py` & `blivet-3.9.2/blivet/devices/storage.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/devices/stratis.py` & `blivet-3.9.2/blivet/devices/stratis.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,16 @@
     _resizable = False
     _packages = ["stratisd", "stratis-cli"]
     _dev_dir = "/dev/stratis"
     _external_dependencies = [availability.STRATISPREDICTUSAGE_APP, availability.STRATIS_DBUS]
     _min_size = Size("512 MiB")
 
     def __init__(self, name, parents=None, size=None, uuid=None, exists=False):
+        if size is None:
+            size = devicelibs.stratis.STRATIS_FS_SIZE
         if not exists and parents[0].free_space <= devicelibs.stratis.filesystem_md_size(size):
             raise StratisError("cannot create new stratis filesystem, not enough free space in the pool")
 
         super(StratisFilesystemDevice, self).__init__(name=name, size=size, uuid=uuid,
                                                       parents=parents, exists=exists)
 
     def _get_name(self):
```

### Comparing `blivet-3.9.1/blivet/devicetree.py` & `blivet-3.9.2/blivet/devicetree.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/errors.py` & `blivet-3.9.2/blivet/errors.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/events/changes.py` & `blivet-3.9.2/blivet/events/changes.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/events/handler.py` & `blivet-3.9.2/blivet/events/handler.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/events/manager.py` & `blivet-3.9.2/blivet/events/manager.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/fcoe.py` & `blivet-3.9.2/blivet/fcoe.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/flags.py` & `blivet-3.9.2/blivet/flags.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/__init__.py` & `blivet-3.9.2/blivet/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/biosboot.py` & `blivet-3.9.2/blivet/formats/biosboot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/disklabel.py` & `blivet-3.9.2/blivet/formats/disklabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/dmraid.py` & `blivet-3.9.2/blivet/formats/dmraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/fs.py` & `blivet-3.9.2/blivet/formats/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from ..tasks import fswritelabel
 from ..tasks import fswriteuuid
 from ..errors import FormatCreateError, FSError, FSReadLabelError
 from ..errors import FSWriteLabelError, FSWriteUUIDError
 from . import DeviceFormat, register_device_format
 from .. import util
 from ..flags import flags
-from ..fstab import FSTabOptions
+from ..fstab import FSTabOptions, HAVE_LIBMOUNT
 from ..storage_log import log_exception_info, log_method_call
 from .. import arch
 from ..size import Size, ROUND_UP
 from ..i18n import N_
 from .. import udev
 from ..mounts import mounts_cache
 from ..devicelibs import btrfs
@@ -698,18 +698,19 @@
             raise FSError("umount of %s failed (%d)" % (mountpoint, rc))
 
         if mountpoint == self._chrooted_mountpoint:
             self._chrooted_mountpoint = None
 
         udev.settle()
 
-    def change_mountpoint(self, dry_run=False):
+    def change_mountpoint(self, dry_run=False):  # pylint: disable=unused-argument
         # This function is intentionally left blank. Mountpoint change utilizes
         # only the generic part of this code branch
-        pass
+        if not HAVE_LIBMOUNT:
+            raise FSError("Fstab management is not supported on this system")
 
     def read_label(self):
         """Read this filesystem's label.
 
            :return: the filesystem's label
            :rtype: str
 
@@ -1090,17 +1091,23 @@
     def is_empty(self):
         """ Check whether this filesystem os empty or not
 
             Note: If the filesystem is not mounted, this will temporarily mount it
                   to a temporary directory.
         """
 
+        def _pre_process_subvolnames(subvols):
+            # subvolumes without the subvolspec prefix (so names are relative to this subvolume)
+            if not self.subvolspec or self.subvolspec == 5:
+                return subvols
+            return [sub[sub.startswith(self.subvolspec + "/") and len(self.subvolspec) + 1:] for sub in subvols]
+
         with self._do_temp_mount() as mnt:
             content = os.listdir(mnt)
-            subvols = btrfs.get_mountpoint_subvolumes(mnt)
+            subvols = _pre_process_subvolnames(btrfs.get_mountpoint_subvolumes(mnt))
             if content and not all(c in self._system_dirs + subvols for c in content):
                 return False
             return True
 
 
 register_device_format(BTRFS)
```

### Comparing `blivet-3.9.1/blivet/formats/fslib.py` & `blivet-3.9.2/blivet/formats/fslib.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/luks.py` & `blivet-3.9.2/blivet/formats/luks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/lvmpv.py` & `blivet-3.9.2/blivet/formats/lvmpv.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/mdraid.py` & `blivet-3.9.2/blivet/formats/mdraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/multipath.py` & `blivet-3.9.2/blivet/formats/multipath.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/prepboot.py` & `blivet-3.9.2/blivet/formats/prepboot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/stratis.py` & `blivet-3.9.2/blivet/formats/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/formats/swap.py` & `blivet-3.9.2/blivet/formats/swap.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/fstab.py` & `blivet-3.9.2/blivet/fstab.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,21 @@
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): Jan Pokorny <japokorn@redhat.com>
 #
 
 import os
 
-from libmount import Table, Fs, MNT_ITER_FORWARD
-from libmount import Error as LibmountException
+try:
+    from libmount import Table, Fs, MNT_ITER_FORWARD
+    from libmount import Error as LibmountException
+except ModuleNotFoundError:
+    HAVE_LIBMOUNT = False
+else:
+    HAVE_LIBMOUNT = True
 
 import logging
 log = logging.getLogger("blivet")
 
 
 class FSTabOptions(object):
     """ User prefered fstab settings object intended to be attached to device.format.
@@ -387,19 +392,56 @@
         else:
             raise ValueError("""cannot generate fstab entry from device '%s' because
                                 it is neither mountable nor swap type""" % device.format.name)
 
         entry.spec = self._get_spec(device)
         if entry.spec is None:
             entry.spec = getattr(device, "fstab_spec", None)
-
         entry.vfstype = device.format.type
 
         return entry
 
+    def entry_from_action(self, action):
+        """ Generate FSTabEntry object based on given blivet Action
+
+            :keyword action: action to process
+            :type action: :class: `blivet.deviceaction.DeviceAction`
+            :returns: fstab entry object based on device processed by action
+            :rtype: :class: `FSTabEntry`
+        """
+
+        if not action.is_format:
+            raise ValueError("""cannot generate fstab entry from action '%s' because
+                                its type is not 'format'""" % action)
+
+        fmt = action.format
+        if action.is_destroy:
+            fmt = action.orig_format
+        if action.is_create:
+            fmt = action.device.format
+
+        entry = FSTabEntry()
+
+        entry.file = None
+        if fmt.mountable:
+            entry.file = fmt.mountpoint
+        elif fmt.type == "swap":
+            entry.file = "swap"
+        else:
+            raise ValueError("""cannot generate fstab entry from action '%s' because
+                                it is neither mountable nor swap type""" % action)
+
+        entry.spec = self._get_spec(action.device)
+        if entry.spec is None:
+            entry.spec = getattr(action.device, "fstab_spec", None)
+
+        entry.vfstype = action.device.format.type
+
+        return entry
+
     def read(self):
         """ Read the fstab file from path stored in self.src_file. Resets currently loaded table contents.
         """
 
         # Reset table
         self._table = Table()
         self._table.enable_comments(True)
@@ -542,15 +584,15 @@
             _entry.file = file
 
         if vfstype is not None:
             _entry.vfstype = vfstype
 
         if mntops is not None:
             _entry.mntops = mntops
-        elif _entry.mntops is None:
+        if _entry.mntops is None:
             _entry.mntops = ['defaults']
 
         if freq is not None:
             # Whether the fs should be dumped by dump(8) (default: 0, i.e. no)
             _entry.freq = freq
         elif _entry.freq is None:
             _entry.freq = 0
@@ -692,15 +734,19 @@
             Returns None if desired spec was not found
         """
 
         # Use device specific spec type if it is set
         # Use "globally" set (on FSTabManager level) spec type otherwise
 
         spec = None
-        spec_type = device.format.fstab.spec_type or self.spec_type
+
+        if hasattr(device.format, 'fstab') and device.format.fstab.spec_type:
+            spec_type = device.format.fstab.spec_type
+        else:
+            spec_type = self.spec_type
 
         if spec_type == "LABEL" and device.format.label:
             spec = "LABEL=%s" % device.format.label
         elif spec_type == "PARTUUID" and device.uuid:
             spec = "PARTUUID=%s" % device.uuid
         elif spec_type == "PARTLABEL" and device.format.name:
             spec = "PARTLABEL=%s" % device.format.name
@@ -733,31 +779,33 @@
             return
 
         if action.is_create and action.is_device and action.device.type == "luks/dm-crypt":
             # when creating luks format, two actions are made. Device creation
             # does not have UUID assigned yet, so we skip that one
             return
 
-        if action.is_create and action.device.format.mountable:
+        if action.is_create and action.is_format and action.device.format.mountable:
             # add the device to the fstab
             # make sure it is not already present there
             try:
                 entry = self.entry_from_device(action.device)
             except ValueError:
                 # this device should not be at fstab
                 found = None
+                entry = None
             else:
                 found = self.find_entry(entry=entry)
 
             # get correct spec type to use (if None, the one already present in entry is used)
             spec = self._get_spec(action.device)
 
             if found is None and action.device.format.mountpoint is not None:
                 # device is not present in fstab and has a defined mountpoint => add it
                 self.add_entry(spec=spec,
+                               file=action.device.format.mountpoint,
                                mntops=action.device.format.fstab.mntops,
                                freq=action.device.format.fstab.freq,
                                passno=action.device.format.fstab.passno,
                                entry=entry)
             elif found and found.spec != spec and action.device.format.mountpoint is not None:
                 # allow change of spec of existing devices
                 self.remove_entry(entry=found)
```

### Comparing `blivet-3.9.1/blivet/i18n.py` & `blivet-3.9.2/blivet/i18n.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/iscsi.py` & `blivet-3.9.2/blivet/iscsi.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/mounts.py` & `blivet-3.9.2/blivet/mounts.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/nvme.py` & `blivet-3.9.2/blivet/nvme.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/partitioning.py` & `blivet-3.9.2/blivet/partitioning.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/__init__.py` & `blivet-3.9.2/blivet/populator/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/boot.py` & `blivet-3.9.2/blivet/populator/helpers/boot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/btrfs.py` & `blivet-3.9.2/blivet/populator/helpers/btrfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/devicepopulator.py` & `blivet-3.9.2/blivet/populator/helpers/devicepopulator.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/disk.py` & `blivet-3.9.2/blivet/populator/helpers/disk.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/disklabel.py` & `blivet-3.9.2/blivet/populator/helpers/disklabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/dm.py` & `blivet-3.9.2/blivet/populator/helpers/dm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/formatpopulator.py` & `blivet-3.9.2/blivet/populator/helpers/formatpopulator.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/loop.py` & `blivet-3.9.2/blivet/populator/helpers/loop.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/luks.py` & `blivet-3.9.2/blivet/populator/helpers/luks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/lvm.py` & `blivet-3.9.2/blivet/populator/helpers/lvm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/mdraid.py` & `blivet-3.9.2/blivet/populator/helpers/mdraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/multipath.py` & `blivet-3.9.2/blivet/populator/helpers/multipath.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/optical.py` & `blivet-3.9.2/blivet/populator/helpers/optical.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/partition.py` & `blivet-3.9.2/blivet/populator/helpers/partition.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/populatorhelper.py` & `blivet-3.9.2/blivet/populator/helpers/populatorhelper.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/helpers/stratis.py` & `blivet-3.9.2/blivet/populator/helpers/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/populator/populator.py` & `blivet-3.9.2/blivet/populator/populator.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/safe_dbus.py` & `blivet-3.9.2/blivet/safe_dbus.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/size.py` & `blivet-3.9.2/blivet/size.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/static_data/luks_data.py` & `blivet-3.9.2/blivet/static_data/luks_data.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/static_data/lvm_info.py` & `blivet-3.9.2/blivet/static_data/lvm_info.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/static_data/mpath_info.py` & `blivet-3.9.2/blivet/static_data/mpath_info.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/static_data/stratis_info.py` & `blivet-3.9.2/blivet/static_data/stratis_info.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/storage_log.py` & `blivet-3.9.2/blivet/storage_log.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/availability.py` & `blivet-3.9.2/blivet/tasks/availability.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import abc
 import shutil
 
 from six import add_metaclass
 
 from .. import safe_dbus
 from ..devicelibs.stratis import STRATIS_SERVICE, STRATIS_PATH
+from .. import util
 
 import gi
 gi.require_version("BlockDev", "3.0")
 gi.require_version("GLib", "2.0")
 gi.require_version("Gio", "2.0")
 
 from gi.repository import BlockDev as blockdev
@@ -313,14 +314,19 @@
 
             :param resource: a DBus service
             :type resource: :class:`ExternalResource`
 
             :returns: [] if the name of the plugin is loaded
             :rtype: list of str
         """
+        # try to start the service first
+        ret = util.run_program(["systemctl", "start", resource.name])
+        if ret != 0:
+            return ["DBus service %s not available" % resource.name]
+
         try:
             avail = blockdev.utils.dbus_service_available(None, Gio.BusType.SYSTEM, self.dbus_name, self.dbus_path)
             avail = safe_dbus.check_object_available(self.dbus_name, self.dbus_path)
         except safe_dbus.DBusCallError:
             return ["DBus service %s not available" % resource.name]
         else:
             if avail:
@@ -491,15 +497,16 @@
 BLOCKDEV_MD_TECH = BlockDevMethod(BLOCKDEV_MD)
 
 # libblockdev mpath plugin required technologies and modes
 BLOCKDEV_MPATH_ALL_MODES = (blockdev.MpathTechMode.MODIFY |
                             blockdev.MpathTechMode.QUERY)
 BLOCKDEV_MPATH = BlockDevTechInfo(plugin_name="mpath",
                                   check_fn=blockdev.mpath_is_tech_avail,
-                                  technologies={blockdev.MpathTech.BASE: BLOCKDEV_MPATH_ALL_MODES})
+                                  technologies={blockdev.MpathTech.BASE: BLOCKDEV_MPATH_ALL_MODES,
+                                                blockdev.MpathTech.FRIENDLY_NAMES: blockdev.MpathTechMode.MODIFY})
 BLOCKDEV_MPATH_TECH = BlockDevMethod(BLOCKDEV_MPATH)
 
 # libblockdev swap plugin required technologies and modes
 BLOCKDEV_SWAP_ALL_MODES = (blockdev.SwapTechMode.CREATE |
                            blockdev.SwapTechMode.ACTIVATE_DEACTIVATE |
                            blockdev.SwapTechMode.QUERY |
                            blockdev.SwapTechMode.SET_LABEL)
@@ -594,8 +601,8 @@
 # other
 KPARTX_APP = application("kpartx")
 MULTIPATH_APP = application("multipath")
 STRATISPREDICTUSAGE_APP = application("stratis-predict-usage")
 
 # dbus services
 STRATIS_SERVICE_METHOD = DBusMethod(STRATIS_SERVICE, STRATIS_PATH)
-STRATIS_DBUS = dbus_service("stratis", STRATIS_SERVICE_METHOD)
+STRATIS_DBUS = dbus_service("stratisd", STRATIS_SERVICE_METHOD)
```

### Comparing `blivet-3.9.1/blivet/tasks/dfresize.py` & `blivet-3.9.2/blivet/tasks/dfresize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsck.py` & `blivet-3.9.2/blivet/tasks/fsck.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsinfo.py` & `blivet-3.9.2/blivet/tasks/fsinfo.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fslabeling.py` & `blivet-3.9.2/blivet/tasks/fslabeling.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsminsize.py` & `blivet-3.9.2/blivet/tasks/fsminsize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsmkfs.py` & `blivet-3.9.2/blivet/tasks/fsmkfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsmount.py` & `blivet-3.9.2/blivet/tasks/fsmount.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsreadlabel.py` & `blivet-3.9.2/blivet/tasks/fsreadlabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsresize.py` & `blivet-3.9.2/blivet/tasks/fsresize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fssize.py` & `blivet-3.9.2/blivet/tasks/fssize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fssync.py` & `blivet-3.9.2/blivet/tasks/fssync.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fstask.py` & `blivet-3.9.2/blivet/tasks/fstask.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fsuuid.py` & `blivet-3.9.2/blivet/tasks/fsuuid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fswritelabel.py` & `blivet-3.9.2/blivet/tasks/fswritelabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/fswriteuuid.py` & `blivet-3.9.2/blivet/tasks/fswriteuuid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/lukstasks.py` & `blivet-3.9.2/blivet/tasks/lukstasks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/pvtask.py` & `blivet-3.9.2/blivet/tasks/pvtask.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tasks/task.py` & `blivet-3.9.2/blivet/tasks/task.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/threads.py` & `blivet-3.9.2/blivet/threads.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/tsort.py` & `blivet-3.9.2/blivet/tsort.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/udev.py` & `blivet-3.9.2/blivet/udev.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet/util.py` & `blivet-3.9.2/blivet/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1161,15 +1161,15 @@
     """ Return True if we are running in a virtual machine. """
     try:
         vm = safe_dbus.get_property_sync(SYSTEMD_SERVICE, SYSTEMD_MANAGER_PATH,
                                          SYSTEMD_MANAGER_IFACE, VIRT_PROP_NAME)
     except (safe_dbus.DBusCallError, safe_dbus.DBusPropertyError):
         return False
     else:
-        return vm[0] in ('qemu', 'kvm', 'xen', 'microsoft')
+        return vm[0] in ('qemu', 'kvm', 'xen', 'microsoft', 'amazon')
 
 
 def natural_sort_key(device):
     """ Sorting key for devices which makes sure partitions are sorted in natural
         way, e.g. 'sda1, sda2, ..., sda10' and not like 'sda1, sda10, sda2, ...'
     """
     if device.type == "partition" and device.parted_partition and device.disk:
```

### Comparing `blivet-3.9.1/blivet/zfcp.py` & `blivet-3.9.2/blivet/zfcp.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/blivet.egg-info/PKG-INFO` & `blivet-3.9.2/blivet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blivet
-Version: 3.9.1
+Version: 3.9.2
 Summary: Python module for system storage configuration
 Home-page: http://github.com/storaged-project/blivet
 Author: David Lehman
 Author-email: dlehman@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `blivet-3.9.1/blivet.egg-info/SOURCES.txt` & `blivet-3.9.2/blivet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/actions.py` & `blivet-3.9.2/examples/actions.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/btrfs.py` & `blivet-3.9.2/examples/btrfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/dbus_client.py` & `blivet-3.9.2/examples/dbus_client.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/factory.py` & `blivet-3.9.2/examples/factory.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm.py` & `blivet-3.9.2/examples/lvm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm_cache.py` & `blivet-3.9.2/examples/lvm_cache.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm_cachepool.py` & `blivet-3.9.2/examples/lvm_cachepool.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm_non_linear.py` & `blivet-3.9.2/examples/lvm_non_linear.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm_thin.py` & `blivet-3.9.2/examples/lvm_thin.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/lvm_vdo.py` & `blivet-3.9.2/examples/lvm_vdo.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/partitioning.py` & `blivet-3.9.2/examples/partitioning.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/stratis.py` & `blivet-3.9.2/examples/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/examples/uevents.py` & `blivet-3.9.2/examples/uevents.py`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/Makefile` & `blivet-3.9.2/po/Makefile`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/af.mo` & `blivet-3.9.2/po/af.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/af.po` & `blivet-3.9.2/po/af.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/am.mo` & `blivet-3.9.2/po/am.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/am.po` & `blivet-3.9.2/po/am.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ar.mo` & `blivet-3.9.2/po/ar.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ar.po` & `blivet-3.9.2/po/ar.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/as.mo` & `blivet-3.9.2/po/as.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/as.po` & `blivet-3.9.2/po/as.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ast.mo` & `blivet-3.9.2/po/ast.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ast.po` & `blivet-3.9.2/po/ast.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bg.mo` & `blivet-3.9.2/po/bg.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bg.po` & `blivet-3.9.2/po/bg.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/blivet.pot` & `blivet-3.9.2/po/blivet.pot`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bn.mo` & `blivet-3.9.2/po/bn.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bn.po` & `blivet-3.9.2/po/bn.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bn_IN.mo` & `blivet-3.9.2/po/bn_IN.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bn_IN.po` & `blivet-3.9.2/po/bn_IN.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bs.mo` & `blivet-3.9.2/po/bs.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/bs.po` & `blivet-3.9.2/po/bs.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ca.mo` & `blivet-3.9.2/po/ca.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ca.po` & `blivet-3.9.2/po/ca.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/cs.mo` & `blivet-3.9.2/po/cs.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/cs.po` & `blivet-3.9.2/po/cs.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/cy.mo` & `blivet-3.9.2/po/cy.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/cy.po` & `blivet-3.9.2/po/cy.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/da.mo` & `blivet-3.9.2/po/da.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/da.po` & `blivet-3.9.2/po/da.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/de.mo` & `blivet-3.9.2/po/de.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/de.po` & `blivet-3.9.2/po/de.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/de_CH.mo` & `blivet-3.9.2/po/de_CH.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/de_CH.po` & `blivet-3.9.2/po/de_CH.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/el.mo` & `blivet-3.9.2/po/el.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/el.po` & `blivet-3.9.2/po/el.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/en_GB.mo` & `blivet-3.9.2/po/en_GB.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/en_GB.po` & `blivet-3.9.2/po/en_GB.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/es.mo` & `blivet-3.9.2/po/es.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/es.po` & `blivet-3.9.2/po/es.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/et.mo` & `blivet-3.9.2/po/et.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/et.po` & `blivet-3.9.2/po/et.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/eu.mo` & `blivet-3.9.2/po/eu.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/eu.po` & `blivet-3.9.2/po/eu.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fa.mo` & `blivet-3.9.2/po/fa.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fa.po` & `blivet-3.9.2/po/fa.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fi.mo` & `blivet-3.9.2/po/fi.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fi.po` & `blivet-3.9.2/po/fi.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fr.mo` & `blivet-3.9.2/po/fr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fr.po` & `blivet-3.9.2/po/fr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fur.mo` & `blivet-3.9.2/po/fur.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/fur.po` & `blivet-3.9.2/po/fur.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/gu.mo` & `blivet-3.9.2/po/gu.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/gu.po` & `blivet-3.9.2/po/gu.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/he.mo` & `blivet-3.9.2/po/he.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/he.po` & `blivet-3.9.2/po/he.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hi.mo` & `blivet-3.9.2/po/hi.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hi.po` & `blivet-3.9.2/po/hi.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hr.mo` & `blivet-3.9.2/po/hr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hr.po` & `blivet-3.9.2/po/hr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hu.mo` & `blivet-3.9.2/po/hu.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/hu.po` & `blivet-3.9.2/po/hu.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ia.mo` & `blivet-3.9.2/po/ia.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ia.po` & `blivet-3.9.2/po/ia.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/id.mo` & `blivet-3.9.2/po/id.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/id.po` & `blivet-3.9.2/po/id.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ilo.mo` & `blivet-3.9.2/po/ilo.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ilo.po` & `blivet-3.9.2/po/ilo.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/is.mo` & `blivet-3.9.2/po/is.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/is.po` & `blivet-3.9.2/po/is.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/it.mo` & `blivet-3.9.2/po/it.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/it.po` & `blivet-3.9.2/po/it.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ja.mo` & `blivet-3.9.2/po/ja.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ja.po` & `blivet-3.9.2/po/ja.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ka.mo` & `blivet-3.9.2/po/ka.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ka.po` & `blivet-3.9.2/po/ka.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/kk.mo` & `blivet-3.9.2/po/kk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/kk.po` & `blivet-3.9.2/po/kk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/kn.mo` & `blivet-3.9.2/po/kn.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/kn.po` & `blivet-3.9.2/po/kn.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ko.mo` & `blivet-3.9.2/po/ko.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ko.po` & `blivet-3.9.2/po/ko.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/lv.mo` & `blivet-3.9.2/po/lv.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/lv.po` & `blivet-3.9.2/po/lv.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mai.mo` & `blivet-3.9.2/po/mai.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mai.po` & `blivet-3.9.2/po/mai.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mk.mo` & `blivet-3.9.2/po/mk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mk.po` & `blivet-3.9.2/po/mk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ml.mo` & `blivet-3.9.2/po/ml.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ml.po` & `blivet-3.9.2/po/ml.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mr.mo` & `blivet-3.9.2/po/mr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/mr.po` & `blivet-3.9.2/po/mr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ms.mo` & `blivet-3.9.2/po/ms.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ms.po` & `blivet-3.9.2/po/ms.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nb.mo` & `blivet-3.9.2/po/nb.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nb.po` & `blivet-3.9.2/po/nb.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ne.mo` & `blivet-3.9.2/po/ne.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ne.po` & `blivet-3.9.2/po/ne.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nl.mo` & `blivet-3.9.2/po/nl.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nl.po` & `blivet-3.9.2/po/nl.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nso.mo` & `blivet-3.9.2/po/nso.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/nso.po` & `blivet-3.9.2/po/nso.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/or.mo` & `blivet-3.9.2/po/or.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/or.po` & `blivet-3.9.2/po/or.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pa.mo` & `blivet-3.9.2/po/pa.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pa.po` & `blivet-3.9.2/po/pa.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pl.mo` & `blivet-3.9.2/po/pl.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pl.po` & `blivet-3.9.2/po/pl.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pt.mo` & `blivet-3.9.2/po/pt.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pt.po` & `blivet-3.9.2/po/pt.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pt_BR.mo` & `blivet-3.9.2/po/pt_BR.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/pt_BR.po` & `blivet-3.9.2/po/pt_BR.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ro.mo` & `blivet-3.9.2/po/ro.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ro.po` & `blivet-3.9.2/po/ro.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ru.mo` & `blivet-3.9.2/po/ru.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ru.po` & `blivet-3.9.2/po/ru.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/si.mo` & `blivet-3.9.2/po/si.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/si.po` & `blivet-3.9.2/po/si.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sk.mo` & `blivet-3.9.2/po/sk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sk.po` & `blivet-3.9.2/po/sk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sl.mo` & `blivet-3.9.2/po/sl.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sl.po` & `blivet-3.9.2/po/sl.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sq.mo` & `blivet-3.9.2/po/sq.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sq.po` & `blivet-3.9.2/po/sq.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sr.mo` & `blivet-3.9.2/po/sr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sr.po` & `blivet-3.9.2/po/sr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sr@latin.mo` & `blivet-3.9.2/po/sr@latin.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sr@latin.po` & `blivet-3.9.2/po/sr@latin.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sv.mo` & `blivet-3.9.2/po/sv.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/sv.po` & `blivet-3.9.2/po/sv.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ta.mo` & `blivet-3.9.2/po/ta.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ta.po` & `blivet-3.9.2/po/ta.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/te.mo` & `blivet-3.9.2/po/te.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/te.po` & `blivet-3.9.2/po/te.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/tg.mo` & `blivet-3.9.2/po/tg.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/tg.po` & `blivet-3.9.2/po/tg.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/th.mo` & `blivet-3.9.2/po/th.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/th.po` & `blivet-3.9.2/po/th.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/tr.mo` & `blivet-3.9.2/po/tr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/tr.po` & `blivet-3.9.2/po/tr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/uk.mo` & `blivet-3.9.2/po/uk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/uk.po` & `blivet-3.9.2/po/uk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ur.mo` & `blivet-3.9.2/po/ur.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/ur.po` & `blivet-3.9.2/po/ur.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/zh_CN.mo` & `blivet-3.9.2/po/zh_CN.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/zh_CN.po` & `blivet-3.9.2/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/zh_TW.mo` & `blivet-3.9.2/po/zh_TW.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/po/zh_TW.po` & `blivet-3.9.2/po/zh_TW.po`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/python-blivet.spec` & `blivet-3.9.2/python-blivet.spec`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Summary:  A python module for system storage configuration
 Name: python-blivet
 Url: https://storageapis.wordpress.com/projects/blivet
-Version: 3.9.1
+Version: 3.9.2
 
 #%%global prerelease .b2
 # prerelease, if defined, should be something like .a1, .b1, .b2.dev1, or .c2
 Release: 1%{?prerelease}%{?dist}
 Epoch: 1
 License: LGPL-2.1-or-later
 %global realname blivet
@@ -106,14 +106,33 @@
 
 %files -n python3-%{realname}
 %license COPYING
 %doc README.md ChangeLog examples
 %{python3_sitelib}/*
 
 %changelog
+* Thu Mar 28 2024 Vojtech Trefny <vtrefny@redhat.com> - 3.9.2-1
+- tests: Add a simple unit test for listing btrfs subvolumes (vtrefny)
+- Fix getting default subvolume ID for mounted btrfs volumes (vtrefny)
+- Do not try to get btrfs subvolumes without libblockdev (vtrefny)
+- Do not raise not implemented exception when checking if btrfs is empty
+  (vtrefny)
+- Try to start stratisd before checking its availability (vtrefny)
+- Fix creating Stratis filesystem without size specified (vtrefny)
+- Fix printing the partition type UUID (vtrefny)
+- Adjust check for btrfs filesystem being empty (vtrefny)
+- Fix util.detect_virt on Amazon (vtrefny)
+- misc: Vagrantfile update (vtrefny)
+- misc: Run pip with --break-system-packages (vtrefny)
+- misc: Add missing libmount build dependencies (vtrefny)
+- availability: Check for mpath friendly names availability (vtrefny)
+- Allow running blivet without libmount Python bindings (vtrefny)
+- Fstab cleanup fix (japokorn)
+- Fix getting subvolumes for mounted btrfs volumes (vtrefny)
+
 * Tue Feb 27 2024 Vojtech Trefny <vtrefny@redhat.com> - 3.9.1-1
 - Try to assemble MD arrays during populate (#2236356) (vtrefny)
 - Fix UnboundLocalError in MD populator (vtrefny)
 - Fix crash when scanning degraded/not fully assembled MD arrays (vtrefny)
 - pylint: Remove some old false positives (vtrefny)
 - tests: Skip MD storage tests on RHEL/CentOS 9 (vtrefny)
 - misc: Bump libblockdev version for Debian (vtrefny)
```

### Comparing `blivet-3.9.1/release_notes.rst` & `blivet-3.9.2/release_notes.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.9.1/setup.py` & `blivet-3.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(name='blivet',
-      version='3.9.1',
+      version='3.9.2',
       cmdclass={"sdist": blivet_sdist},
       description='Python module for system storage configuration',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='David Lehman', author_email='dlehman@redhat.com',
       url='http://github.com/storaged-project/blivet',
       data_files=data_files,
```

