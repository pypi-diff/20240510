# Comparing `tmp/dimples-0.5.8.tar.gz` & `tmp/dimples-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.5.8.tar", last modified: Wed Apr 24 10:21:32 2024, max compression
+gzip compressed data, was "dist/dimples-1.0.0.tar", last modified: Fri May 10 15:58:45 2024, max compression
```

## Comparing `dimples-0.5.8.tar` & `dimples-1.0.0.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-24 10:21:32.000000 dimples-0.5.8/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.8/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.8/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.8/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.8/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-0.5.8/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.8/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.8/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.8/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.8/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.8/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.8/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.8/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.8/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.8/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.8/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.8/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.8/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.8/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.8/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.8/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6624 2024-04-23 08:44:53.000000 dimples-0.5.8/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8638 2024-04-23 09:37:33.000000 dimples-0.5.8/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.8/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.8/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.8/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5560 2024-04-23 08:43:31.000000 dimples-0.5.8/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.8/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.8/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.8/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.8/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.8/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.8/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.8/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.8/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.8/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.8/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.8/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.8/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.8/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7937 2024-04-23 09:37:33.000000 dimples-0.5.8/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.8/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-24 03:34:20.000000 dimples-0.5.8/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.8/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.8/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.8/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.8/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.8/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.8/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.8/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.8/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.8/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.8/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4561 2024-04-23 09:37:33.000000 dimples-0.5.8/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.8/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.8/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    11821 2024-04-24 03:33:28.000000 dimples-0.5.8/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.8/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.8/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.8/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-0.5.8/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.8/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-0.5.8/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.8/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     4207 2024-04-24 03:37:25.000000 dimples-0.5.8/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.8/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.8/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.8/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.8/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.8/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.8/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.8/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.8/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.8/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.8/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.8/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.8/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.8/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.8/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.8/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.8/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.8/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.8/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.8/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.8/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.8/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.8/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.8/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.8/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.8/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.8/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.8/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.8/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    15767 2024-04-24 10:12:35.000000 dimples-0.5.8/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.8/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.8/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.8/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.8/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.8/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.8/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.8/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.8/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.8/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.8/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-24 08:01:26.000000 dimples-0.5.8/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.8/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.8/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.8/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.8/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.8/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7406 2024-04-24 04:11:06.000000 dimples-0.5.8/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.8/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.8/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.8/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.8/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.8/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.8/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    17519 2024-04-24 10:12:35.000000 dimples-0.5.8/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4454 2024-04-23 10:00:05.000000 dimples-0.5.8/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-24 03:35:15.000000 dimples-0.5.8/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    13850 2024-04-24 05:59:48.000000 dimples-0.5.8/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5476 2024-04-23 08:44:27.000000 dimples-0.5.8/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9843 2024-04-24 03:38:06.000000 dimples-0.5.8/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.8/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.8/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.8/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3832 2024-04-22 16:08:14.000000 dimples-0.5.8/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.8/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.8/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4710 2024-04-23 08:43:02.000000 dimples-0.5.8/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6355 2024-04-23 08:38:51.000000 dimples-0.5.8/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-0.5.8/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.8/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.8/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.8/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-24 10:21:32.000000 dimples-0.5.8/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-24 10:21:32.000000 dimples-0.5.8/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-24 10:13:20.000000 dimples-0.5.8/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-10 15:58:45.000000 dimples-1.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.0.0/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.0.0/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.0.0/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.0.0/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.0.0/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.0.0/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.0.0/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.0.0/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.0.0/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.0.0/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.0.0/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.0.0/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.0.0/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.0.0/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.0.0/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.0.0/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.0.0/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.0.0/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.0.0/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.0.0/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     9331 2024-05-09 16:38:52.000000 dimples-1.0.0/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.0.0/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.0.0/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.0.0/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5525 2024-05-09 19:49:02.000000 dimples-1.0.0/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.0.0/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.0.0/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.0.0/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.0.0/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.0.0/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.0.0/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.0.0/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.0.0/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.0.0/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.0.0/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.0.0/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.0.0/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.0.0/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     8007 2024-05-06 18:03:43.000000 dimples-1.0.0/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.0.0/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.0.0/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.0.0/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.0.0/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.0.0/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.0.0/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.0.0/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.0.0/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.0.0/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.0.0/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.0.0/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.0.0/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.0.0/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-1.0.0/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10934 2024-05-07 17:49:30.000000 dimples-1.0.0/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12254 2024-05-10 05:26:49.000000 dimples-1.0.0/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10800 2024-05-07 16:01:10.000000 dimples-1.0.0/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7992 2024-05-07 16:02:25.000000 dimples-1.0.0/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.0.0/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-1.0.0/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-1.0.0/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.0.0/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     4261 2024-05-07 18:47:41.000000 dimples-1.0.0/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7910 2024-05-09 16:38:10.000000 dimples-1.0.0/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.0.0/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.0.0/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.0.0/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-1.0.0/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.0.0/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.0.0/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.0.0/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.0.0/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.0.0/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.0.0/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.0.0/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.0.0/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.0.0/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.0.0/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.0.0/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.0.0/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.0.0/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.0.0/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.0.0/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.0.0/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.0.0/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.0.0/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.0.0/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    16034 2024-05-09 19:52:12.000000 dimples-1.0.0/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6071 2024-05-07 17:55:00.000000 dimples-1.0.0/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2848 2024-05-10 14:43:14.000000 dimples-1.0.0/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.0.0/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.0.0/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.0.0/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.0.0/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.0.0/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5275 2024-05-06 18:58:53.000000 dimples-1.0.0/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.0.0/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.0.0/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.0.0/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.0.0/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.0.0/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3910 2024-05-09 16:40:41.000000 dimples-1.0.0/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.0.0/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.0.0/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.0.0/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.0.0/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.0.0/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.0.0/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.0.0/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.0.0/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.0.0/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    17669 2024-05-09 19:47:47.000000 dimples-1.0.0/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.0.0/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.0.0/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.0.0/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5453 2024-05-09 19:53:21.000000 dimples-1.0.0/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)    10034 2024-05-10 14:19:20.000000 dimples-1.0.0/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.0.0/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.0.0/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3029 2024-05-10 14:24:22.000000 dimples-1.0.0/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7433 2024-05-07 17:52:09.000000 dimples-1.0.0/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.0.0/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4740 2024-05-09 19:46:27.000000 dimples-1.0.0/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6511 2024-05-10 05:25:44.000000 dimples-1.0.0/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.0.0/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.0.0/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3982 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:58:45.000000 dimples-1.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-10 15:51:37.000000 dimples-1.0.0/setup.py
```

### Comparing `dimples-0.5.8/PKG-INFO` & `dimples-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.8
+Version: 1.0.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.8/README.md` & `dimples-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/__init__.py` & `dimples-1.0.0/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/__init__.py` & `dimples-1.0.0/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/archivist.py` & `dimples-1.0.0/dimples/client/archivist.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,173 +71,173 @@
     def is_documents_respond_expired(self, identifier: ID, force: bool) -> bool:
         return self.__document_responses.is_expired(key=identifier, force=force)
 
     def set_last_active_member(self, member: ID, group: ID):
         self.__last_active_members[group] = member
 
     # Override
-    def query_meta(self, identifier: ID) -> bool:
+    async def query_meta(self, identifier: ID) -> bool:
         if not self.is_meta_query_expired(identifier=identifier):
             # query not expired yet
             self.info(msg='meta query not expired yet: %s' % identifier)
             return False
         messenger = get_messenger(archivist=self)
         if messenger is None:
             self.warning(msg='messenger not ready yet')
             return False
         self.info(msg='querying meta for: %s' % identifier)
         command = MetaCommand.query(identifier=identifier)
-        _, r_msg = messenger.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
+        _, r_msg = await messenger.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
         return r_msg is not None
 
     # Override
-    def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    async def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
         if not self.is_documents_query_expired(identifier=identifier):
             # query not expired yet
             self.info(msg='document query not expired yet: %s' % identifier)
             return False
         messenger = get_messenger(archivist=self)
         if messenger is None:
             self.warning(msg='messenger not ready yet')
             return False
-        last_time = self.get_last_document_time(identifier=identifier, documents=documents)
+        last_time = await self.get_last_document_time(identifier=identifier, documents=documents)
         self.info(msg='querying document for: %s, last time: %s' % (identifier, last_time))
         command = DocumentCommand.query(identifier=identifier, last_time=last_time)
-        _, r_msg = messenger.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
+        _, r_msg = await messenger.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
         return r_msg is not None
 
     # Override
-    def query_members(self, group: ID, members: List[ID]) -> bool:
+    async def query_members(self, group: ID, members: List[ID]) -> bool:
         if not self.is_members_query_expired(group=group):
             # query not expired yet
             self.info('members query not expired yet: %s' % group)
             return False
         facebook = get_facebook(archivist=self)
         messenger = get_messenger(archivist=self)
         if facebook is None or messenger is None:
             self.warning(msg='facebook messenger not ready yet')
             return False
         user = facebook.current_user
         if user is None:
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
-        last_time = self.get_last_group_history_time(group=group)
+        last_time = await self.get_last_group_history_time(group=group)
         self.info(msg='querying members for group: %s, last time: %s' % (group, last_time))
         # build query command for group members
         command = GroupCommand.query(group=group, last_time=last_time)
         # 1. check group bots
-        ok = self.query_members_from_assistants(command=command, sender=me, group=group)
+        ok = await self.query_members_from_assistants(command=command, sender=me, group=group)
         if ok:
             return True
         # 2. check administrators
-        ok = self.query_members_from_administrators(command=command, sender=me, group=group)
+        ok = await self.query_members_from_administrators(command=command, sender=me, group=group)
         if ok:
             return True
         # 3. check group owner
-        ok = self.query_members_from_owner(command=command, sender=me, group=group)
+        ok = await self.query_members_from_owner(command=command, sender=me, group=group)
         if ok:
             return True
         # all failed, try last active member
         last_member = self.__last_active_members.get(group)
         if last_member is None:
             r_msg = None
         else:
             self.info(msg='querying members from: %s, group: %s' % (last_member, group))
-            _, r_msg = messenger.send_content(sender=me, receiver=last_member, content=command, priority=1)
+            _, r_msg = await messenger.send_content(sender=me, receiver=last_member, content=command, priority=1)
         self.error(msg='group not ready: %s' % group)
         return r_msg is not None
 
     # protected
-    def query_members_from_assistants(self, command: QueryCommand, sender: ID, group: ID) -> bool:
+    async def query_members_from_assistants(self, command: QueryCommand, sender: ID, group: ID) -> bool:
         facebook = get_facebook(archivist=self)
         messenger = get_messenger(archivist=self)
         if facebook is None or messenger is None:
             self.warning(msg='facebook messenger not ready yet')
             return False
-        bots = facebook.assistants(group)
+        bots = await facebook.get_assistants(group)
         if len(bots) == 0:
             self.warning(msg='assistants not designated for group: %s' % group)
             return False
         success = 0
         # querying members from bots
         self.info(msg='querying members from bots: %s, group: %s' % (bots, group))
         for receiver in bots:
             if receiver == sender:
                 self.warning(msg='ignore cycled querying: %s, group: %s' % (receiver, group))
                 continue
-            _, r_msg = messenger.send_content(sender=sender, receiver=receiver, content=command, priority=1)
+            _, r_msg = await messenger.send_content(sender=sender, receiver=receiver, content=command, priority=1)
             if r_msg is not None:
                 success += 1
         if success == 0:
             # failed
             return False
         last_member = self.__last_active_members.get(group)
         if last_member is None or last_member in bots:
             # last active member is a bot??
             pass
         else:
             self.info(msg='querying members from: %s, group: %s' % (last_member, group))
-            messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
+            await messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
         return True
 
     # protected
-    def query_members_from_administrators(self, command: QueryCommand, sender: ID, group: ID) -> bool:
+    async def query_members_from_administrators(self, command: QueryCommand, sender: ID, group: ID) -> bool:
         facebook = get_facebook(archivist=self)
         messenger = get_messenger(archivist=self)
         if facebook is None or messenger is None:
             self.warning(msg='facebook messenger not ready yet')
             return False
-        admins = facebook.administrators(group)
+        admins = await facebook.get_administrators(group)
         if len(admins) == 0:
             self.warning(msg='administrators not found for group: %s' % group)
             return False
         success = 0
         # querying members from admins
         self.info(msg='querying members from admins: %s, group: %s' % (admins, group))
         for receiver in admins:
             if receiver == sender:
                 self.warning(msg='ignore cycled querying: %s, group: %s' % (receiver, group))
                 continue
-            _, r_msg = messenger.send_content(sender=sender, receiver=receiver, content=command, priority=1)
+            _, r_msg = await messenger.send_content(sender=sender, receiver=receiver, content=command, priority=1)
             if r_msg is not None:
                 success += 1
         if success == 0:
             # failed
             return False
         last_member = self.__last_active_members.get(group)
         if last_member is None or last_member in admins:
             # last active member is an admin, already queried
             pass
         else:
             self.info(msg='querying members from: %s, group: %s' % (last_member, group))
-            messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
+            await messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
         return True
 
     # protected
-    def query_members_from_owner(self, command: QueryCommand, sender: ID, group: ID) -> bool:
+    async def query_members_from_owner(self, command: QueryCommand, sender: ID, group: ID) -> bool:
         facebook = get_facebook(archivist=self)
         messenger = get_messenger(archivist=self)
         if facebook is None or messenger is None:
             self.warning(msg='facebook messenger not ready yet')
             return False
-        owner = facebook.owner(group)
+        owner = await facebook.get_owner(group)
         if owner is None:
             self.warning(msg='owner not found for group: %s' % group)
             return False
         elif owner == sender:
             self.error(msg='you are the owner of group: %s' % group)
             return False
         # querying members from owner
         self.info(msg='querying members from owner: %s, group: %s' % (owner, group))
-        _, r_msg = messenger.send_content(sender=sender, receiver=owner, content=command, priority=1)
+        _, r_msg = await messenger.send_content(sender=sender, receiver=owner, content=command, priority=1)
         if r_msg is None:
             # failed
             return False
         last_member = self.__last_active_members.get(group)
         if last_member is None or last_member == owner:
             # last active member is the owner, already queried
             pass
         else:
             self.info(msg='querying members from: %s, group: %s' % (last_member, group))
-            messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
+            await messenger.send_content(sender=sender, receiver=last_member, content=command, priority=1)
         return True
```

### Comparing `dimples-0.5.8/dimples/client/checkpoint.py` & `dimples-1.0.0/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/cpu/__init__.py` & `dimples-1.0.0/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/cpu/commands.py` & `dimples-1.0.0/dimples/client/cpu/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 from ...common import LoginCommand
 
 
 class LoginCommandProcessor(BaseCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, LoginCommand), 'login command error: %s' % content
         # return ReceiptCommand.new(message='Login received')
         return []
 
 
 # TODO: AnsCommandProcessor
```

### Comparing `dimples-0.5.8/dimples/client/cpu/creator.py` & `dimples-1.0.0/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/cpu/group.py` & `dimples-1.0.0/dimples/client/cpu/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
         assert isinstance(transceiver, CommonMessenger), 'transceiver error: %s' % transceiver
         return transceiver
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, Command), 'history command error: %s' % content
         text = 'Command not support.'
         return self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
             'template': 'History command (name: ${command}) not support yet!',
             'replacements': {
                 'command': content.cmd,
             }
@@ -119,57 +119,57 @@
     def _create_builder(self) -> GroupHistoryBuilder:
         """ override for customized builder """
         return GroupHistoryBuilder(delegate=self.delegate)
 
 
 class GroupCommandProcessor(HistoryCommandProcessor):
 
-    def _owner(self, group: ID) -> Optional[ID]:
+    async def _owner(self, group: ID) -> Optional[ID]:
         delegate = self.delegate
-        return delegate.owner(identifier=group)
+        return await delegate.get_owner(identifier=group)
 
-    def _assistants(self, group: ID) -> List[ID]:
+    async def _assistants(self, group: ID) -> List[ID]:
         delegate = self.delegate
-        return delegate.assistants(identifier=group)
+        return await delegate.get_assistants(identifier=group)
 
-    def _administrators(self, group: ID) -> List[ID]:
+    async def _administrators(self, group: ID) -> List[ID]:
         delegate = self.delegate
-        return delegate.administrators(group=group)
+        return await delegate.get_administrators(group=group)
 
-    def _save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def _save_administrators(self, administrators: List[ID], group: ID) -> bool:
         delegate = self.delegate
-        return delegate.save_administrators(administrators=administrators, group=group)
+        return await delegate.save_administrators(administrators=administrators, group=group)
 
-    def _members(self, group: ID) -> List[ID]:
+    async def _members(self, group: ID) -> List[ID]:
         delegate = self.delegate
-        return delegate.members(identifier=group)
+        return await delegate.get_members(identifier=group)
 
-    def _save_members(self, members: List[ID], group: ID) -> bool:
+    async def _save_members(self, members: List[ID], group: ID) -> bool:
         delegate = self.delegate
-        return delegate.save_members(members=members, group=group)
+        return await delegate.save_members(members=members, group=group)
 
-    def _save_group_history(self, group: ID, content: GroupCommand, r_msg: ReliableMessage) -> bool:
+    async def _save_group_history(self, group: ID, content: GroupCommand, r_msg: ReliableMessage) -> bool:
         delegate = self.helper
-        return delegate.save_group_history(group=group, content=content, message=r_msg)
+        return await delegate.save_group_history(group=group, content=content, message=r_msg)
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, GroupCommand), 'group command error: %s' % content
         text = 'Command not support.'
         return self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
             'template': 'Group command (name: ${command}) not support yet!',
             'replacements': {
                 'command': content.cmd,
             }
         })
 
-    def _check_expired(self, content: GroupCommand, r_msg: ReliableMessage) -> Tuple[Optional[ID], List[Content]]:
+    async def _check_expired(self, content: GroupCommand, r_msg: ReliableMessage) -> Tuple[Optional[ID], List[Content]]:
         group = content.group
         assert group is not None, 'group command error: %s' % content
-        expired = self.helper.is_expired(content=content)
+        expired = await self.helper.is_expired(content=content)
         if expired:
             text = 'Command expired.'
             errors = self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
                 'template': 'Group command expired: ${cmd}, group: ${ID}.',
                 'replacements': {
                     'cmd': content.cmd,
                     'ID': str(group),
@@ -177,15 +177,16 @@
             })
             group = None
         else:
             # group ID must not empty here
             errors = None
         return group, errors
 
-    def _check_command_members(self, content: GroupCommand, r_msg: ReliableMessage) -> Tuple[List[ID], List[Content]]:
+    async def _check_command_members(self, content: GroupCommand, r_msg: ReliableMessage
+                                     ) -> Tuple[List[ID], List[Content]]:
         group = content.group
         assert group is not None, 'group command error: %s' % content
         members = self.helper.members_from_command(content=content)
         if len(members) == 0:
             text = 'Command error.'
             errors = self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
                 'template': 'Group members empty: ${ID}.',
@@ -194,20 +195,20 @@
                 }
             })
         else:
             # normally
             errors = None
         return members, errors
 
-    def _check_group_members(self, content: GroupCommand,
-                             r_msg: ReliableMessage) -> Tuple[Optional[ID], List[ID], List[Content]]:
+    async def _check_group_members(self, content: GroupCommand, r_msg: ReliableMessage
+                                   ) -> Tuple[Optional[ID], List[ID], List[Content]]:
         group = content.group
         assert group is not None, 'group command error: %s' % content
-        owner = self._owner(group=group)
-        members = self._members(group=group)
+        owner = await self._owner(group=group)
+        members = await self._members(group=group)
         if owner is None or len(members) == 0:
             # TODO: query group members?
             text = 'Group empty.'
             errors = self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
                 'template': 'Group empty: ${ID}.',
                 'replacements': {
                     'ID': str(group),
@@ -215,15 +216,15 @@
             })
         else:
             # group is ready
             errors = None
         return owner, members, errors
 
     # protected
-    def send_group_histories(self, group: ID, receiver: ID) -> bool:
-        messages = self.builder.build_group_histories(group=group)
+    async def send_group_histories(self, group: ID, receiver: ID) -> bool:
+        messages = await self.builder.build_group_histories(group=group)
         if len(messages) == 0:
             self.warning(msg='failed to build history for group: %s' % group)
             return False
         content = ForwardContent.create(messages=messages)
-        _, r_msg = self.messenger.send_content(sender=None, receiver=receiver, content=content, priority=1)
+        _, r_msg = await self.messenger.send_content(sender=None, receiver=receiver, content=content, priority=1)
         return r_msg is not None
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_expel.py` & `dimples-1.0.0/dimples/client/cpu/grp_expel.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,14 @@
 
 from .group import GroupCommandProcessor
 
 
 class ExpelCommandProcessor(GroupCommandProcessor, Logging):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ExpelCommand), 'expel command error: %s' % content
 
         self.warning(msg='"expel" group command is deprecated, use "reset" instead.')
 
         # no need to response this group command
         return []
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_invite.py` & `dimples-1.0.0/dimples/client/cpu/grp_invite.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,37 +46,37 @@
 
 from .group import GroupCommandProcessor
 
 
 class InviteCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, InviteCommand), 'invite command error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
-        invite_list, errors = self._check_command_members(content=content, r_msg=r_msg)
+        invite_list, errors = await self._check_command_members(content=content, r_msg=r_msg)
         if len(invite_list) == 0:
             # command error
             return errors
 
         # 1. check group
-        trip = self._check_group_members(content=content, r_msg=r_msg)
+        trip = await self._check_group_members(content=content, r_msg=r_msg)
         owner = trip[0]
         members = trip[1]
         errors = trip[2]
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        admins = self._administrators(group=group)
+        admins = await self._administrators(group=group)
         is_owner = sender == owner
         is_admin = sender in admins
         is_member = sender in members
         can_reset = is_owner or is_admin
         cannot_reset = not can_reset
 
         # 2. check permission
@@ -96,25 +96,25 @@
             # but if it can still receive an 'invite' command here,
             # we should respond the sender with the newest membership again.
             user = self.facebook.current_user
             if cannot_reset and owner == user.identifier:
                 # the sender cannot reset the group, means it's an ordinary member now,
                 # and if I am the owner, then send the group history commands
                 # to update the sender's memory.
-                ok = self.send_group_histories(group=group, receiver=sender)
+                ok = await self.send_group_histories(group=group, receiver=sender)
                 assert ok, 'failed to send history for group: %s => %s' % (group, sender)
-        elif not self._save_group_history(group=group, content=content, r_msg=r_msg):
+        elif not await self._save_group_history(group=group, content=content, r_msg=r_msg):
             # here try to append the 'invite' command to local storage as group history
             # it should not failed unless the command is expired
             self.error(msg='failed to save "invite" command for group: %s' % group)
         elif cannot_reset:
             # the sender cannot reset the group, means it's invited by ordinary member,
             # and the 'invite' command was saved, now waiting for review.
             self.info(msg='"invite" command saved, waiting review now')
-        elif self._save_members(members=new_members, group=group):
+        elif await self._save_members(members=new_members, group=group):
             # FIXME: this sender has permission to reset the group,
             #        means it must be the owner or an administrator,
             #        usually it should send a 'reset' command instead;
             #        if we received the 'invite' command here, maybe it was confused,
             #        anyway, we just append the new members directly.
             self.warning(msg='invited by administrator: %s, group: %s' % (sender, group))
             content['added'] = ID.revert(added_list)
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_join.py` & `dimples-1.0.0/dimples/client/cpu/grp_join.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
 from .group import GroupCommandProcessor
 
 
 class JoinCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, JoinCommand), 'join command error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
 
         # 1. check group
-        owner, members, errors = self._check_group_members(content=content, r_msg=r_msg)
+        owner, members, errors = await self._check_group_members(content=content, r_msg=r_msg)
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        admins = self._administrators(group=group)
+        admins = await self._administrators(group=group)
         is_owner = sender == owner
         is_admin = sender in admins
         is_member = sender in members
         can_reset = is_owner or is_admin
         cannot_reset = not can_reset
 
         # 2. check membership
@@ -76,17 +76,17 @@
             # but if it can still receive a 'join' command here,
             # we should notify the sender that the member list was updated.
             user = self.facebook.current_user
             if cannot_reset and owner == user.identifier:
                 # the sender cannot reset the group, means it's an ordinary member now,
                 # and if I am the owner, then send the group history commands
                 # to update the sender's memory.
-                ok = self.send_group_histories(group=group, receiver=sender)
+                ok = await self.send_group_histories(group=group, receiver=sender)
                 assert ok, 'failed to send history for group: %s => %s' % (group, sender)
-        elif not self._save_group_history(group=group, content=content, r_msg=r_msg):
+        elif not await self._save_group_history(group=group, content=content, r_msg=r_msg):
             # here try to append the 'join' command to local storage as group history
             # it should not failed unless the command is expired
             self.error(msg='failed to save "join" command for group: %s' % group)
         else:
             # the 'join' command was saved, now waiting for review.
             self.info(msg='"join" command saved, waiting review now')
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_query.py` & `dimples-1.0.0/dimples/client/cpu/grp_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
 from .group import GroupCommandProcessor
 
 
 class QueryCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, QueryCommand), 'query command error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
 
         # 1. check group
-        owner, members, errors = self._check_group_members(content=content, r_msg=r_msg)
+        owner, members, errors = await self._check_group_members(content=content, r_msg=r_msg)
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        bots = self._assistants(group=group)
+        bots = await self._assistants(group=group)
         is_member = sender in members
         is_bot = sender in bots
         can_query = is_member or is_bot
 
         # 2. check permission
         if not can_query:
             text = 'Permission denied.'
@@ -79,27 +79,27 @@
             })
 
         # check last group time
         query_time = content.last_time
         if query_time is not None:
             # check last group history time
             archivist = self.facebook.archivist
-            last_time = archivist.get_last_group_history_time(group=group)
+            last_time = await archivist.get_last_group_history_time(group=group)
             if last_time is None:
                 self.error(msg='group history error: %s' % group)
             elif not last_time.after(query_time):
                 # group history not updated
                 text = 'Group history not updated.'
                 return self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
                     'template': 'Group history not updated: ${ID}, last time: ${time}',
                     'replacements': {
                         'ID': str(group),
                         'time': last_time.timestamp,
                     }
                 })
 
         # 3. send newest group history commands
-        ok = self.send_group_histories(group=group, receiver=sender)
+        ok = await self.send_group_histories(group=group, receiver=sender)
         assert ok, 'failed to send history for group: %s => %s' % (group, sender)
 
         # no need to response this group command
         return []
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_quit.py` & `dimples-1.0.0/dimples/client/cpu/grp_quit.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
 from .group import GroupCommandProcessor
 
 
 class QuitCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, QuitCommand), 'quit command error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
 
         # 1. check group
-        owner, members, errors = self._check_group_members(content=content, r_msg=r_msg)
+        owner, members, errors = await self._check_group_members(content=content, r_msg=r_msg)
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        admins = self._administrators(group=group)
+        admins = await self._administrators(group=group)
         is_owner = sender == owner
         is_admin = sender in admins
         is_member = sender in members
 
         # 2. check permission
         if is_owner:
             text = 'Permission denied.'
@@ -91,19 +91,19 @@
             members = new_members
 
         # 3. do quit
         if not is_member:
             # the sender is not a member now,
             # shall we notify the sender that the member list was updated?
             self.warning(msg='not a member now: %s, %s' % (sender, group))
-        elif not self._save_group_history(group=group, content=content, r_msg=r_msg):
+        elif not await self._save_group_history(group=group, content=content, r_msg=r_msg):
             # here try to append the 'quit' command to local storage as group history
             # it should not failed unless the command is expired
             self.error(msg='failed to save "quit" command for group: %s' % group)
-        elif self._save_members(members=members, group=group):
+        elif await self._save_members(members=members, group=group):
             # here try to remove the sender from member list
             content['removed'] = [str(sender)]
         else:
             # DB error?
             assert False, 'failed to save members for group: %s' % group
 
         # no need to response this group command
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_reset.py` & `dimples-1.0.0/dimples/client/cpu/grp_reset.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,34 +45,34 @@
 
 from .group import GroupCommandProcessor
 
 
 class ResetCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ResetCommand), 'group cmd error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
-        new_members, errors = self._check_command_members(content=content, r_msg=r_msg)
+        new_members, errors = await self._check_command_members(content=content, r_msg=r_msg)
         if len(new_members) == 0:
             # command error
             return errors
 
         # 1. check group
-        owner, members, errors = self._check_group_members(content=content, r_msg=r_msg)
+        owner, members, errors = await self._check_group_members(content=content, r_msg=r_msg)
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        administrators = self._administrators(group=group)
+        administrators = await self._administrators(group=group)
         is_owner = sender == owner
         is_admin = sender in administrators
 
         # 2. check permission
         can_reset = is_owner or is_admin
         if not can_reset:
             text = 'Permission denied.'
@@ -104,22 +104,22 @@
                 'replacements': {
                     'ID': str(group),
                 }
             })
 
         # 3. do reset
         add_list, remove_list = calculate_reset(old_members=members, new_members=new_members)
-        if not self._save_group_history(group=group, content=content, r_msg=r_msg):
+        if not await self._save_group_history(group=group, content=content, r_msg=r_msg):
             # here try to save the 'reset' command to local storage as group history
             # it should not failed unless the command is expired
             self.error(msg='failed to save "reset" command for group: %s' % group)
         elif len(add_list) == 0 and len(remove_list) == 0:
             # nothing changed
             self.warning(msg='nothing changed for group members: %d, %s' % (len(members), group))
-        elif self._save_members(members=new_members, group=group):
+        elif await self._save_members(members=new_members, group=group):
             self.info(msg='new members saved in group: %s' % group)
             if len(add_list) > 0:
                 content['added'] = ID.revert(add_list)
             if len(remove_list) > 0:
                 content['removed'] = ID.revert(remove_list)
         else:
             # DB error?
```

### Comparing `dimples-0.5.8/dimples/client/cpu/grp_resign.py` & `dimples-1.0.0/dimples/client/cpu/grp_resign.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
 from .group import GroupCommandProcessor
 
 
 class ResignCommandProcessor(GroupCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ResignCommand), 'resign command error: %s' % content
 
         # 0. check command
-        group, errors = self._check_expired(content=content, r_msg=r_msg)
+        group, errors = await self._check_expired(content=content, r_msg=r_msg)
         if group is None:
             # ignore expired command
             return errors
 
         # 1. check group
-        owner, members, errors = self._check_group_members(content=content, r_msg=r_msg)
+        owner, members, errors = await self._check_group_members(content=content, r_msg=r_msg)
         if owner is None or len(members) == 0:
             return errors
 
         sender = r_msg.sender
-        admins = self._administrators(group=group)
+        admins = await self._administrators(group=group)
         is_owner = sender == owner
         is_admin = sender in admins
 
         # 2. check permission
         if is_owner:
             text = 'Permission denied.'
             return self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
@@ -82,19 +82,19 @@
             admins = new_admins
 
         # 3. do resign
         if not is_admin:
             # the sender is not an administrator now,
             # shall we notify the sender that the administrators list was updated?
             self.warning(msg='not an administrator now: %s, %s' % (sender, group))
-        elif not self._save_group_history(group=group, content=content, r_msg=r_msg):
+        elif not await self._save_group_history(group=group, content=content, r_msg=r_msg):
             # here try to append the 'resign' command to local storage as group history
             # it should not failed unless the command is expired
             self.error(msg='failed to save "resign" command for group: %s' % group)
-        elif self._save_administrators(administrators=admins, group=group):
+        elif await self._save_administrators(administrators=admins, group=group):
             # here try to remove the sender from admin list
             content['removed'] = [str(sender)]
         else:
             # DB error?
             assert False, 'failed to save members for group: %s' % group
 
         # no need to response this group command
```

### Comparing `dimples-0.5.8/dimples/client/cpu/handshake.py` & `dimples-1.0.0/dimples/client/cpu/handshake.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from ...utils import Logging
 from ...common import HandshakeCommand
 
 
 class HandshakeCommandProcessor(BaseCommandProcessor, Logging):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, HandshakeCommand), 'handshake command error: %s' % content
         messenger = get_client_messenger(cpu=self)
         client_session = get_client_session(messenger=messenger)
         # update station's default ID ('station@anywhere') to sender (real ID)
         station = client_session.station
         oid = station.identifier
         sender = r_msg.sender
@@ -64,20 +64,20 @@
         assert new_sess_key is not None, 'new session key should not be empty: %s' % content
         if 'DIM?' == title:
             # S -> C: station ask client to handshake again
             self.info(msg='handshake again, session key: %s' % new_sess_key)
             # clear client session key while handshake again
             if old_sess_key is None:
                 # first handshake response with new session key,
-                messenger.handshake(session_key=new_sess_key)
+                await messenger.handshake(session_key=new_sess_key)
             elif old_sess_key == new_sess_key:
                 # duplicated handshake response?
                 # or session expired and the station ask to handshake again?
                 self.warning(msg='session key already set: %s => %s' % (old_sess_key, new_sess_key))
-                messenger.handshake(session_key=new_sess_key)
+                await messenger.handshake(session_key=new_sess_key)
             else:
                 # connection changed?
                 self.error(msg='session key from %s not match: %s => %s' % (sender, old_sess_key, new_sess_key))
                 # erase session key to handshake again
                 client_session.key = None
         elif 'DIM!' == title:
             # S -> C: handshake accepted by station
```

### Comparing `dimples-0.5.8/dimples/client/facebook.py` & `dimples-1.0.0/dimples/client/facebook.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,135 +38,135 @@
 
 from ..common import CommonFacebook
 
 
 class ClientFacebook(CommonFacebook):
 
     # Override
-    def save_document(self, document: Document) -> bool:
-        ok = super().save_document(document=document)
+    async def save_document(self, document: Document) -> bool:
+        ok = await super().save_document(document=document)
         if ok and isinstance(document, Bulletin):
             # check administrators
             array = document.get_property(key='administrators')
             if array is not None:
                 group = document.identifier
                 assert group.is_group, 'group ID error: %s' % group
                 admins = ID.convert(array=array)
-                ok = self.save_administrators(administrators=admins, group=group)
+                ok = await self.save_administrators(administrators=admins, group=group)
         return ok
 
     #
     #   GroupDataSource
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
+    async def get_founder(self, identifier: ID) -> Optional[ID]:
         # check broadcast group
         if identifier.is_broadcast:
             # founder of broadcast group
             return BroadcastHelper.broadcast_founder(group=identifier)
         # check bulletin document
-        doc = self.bulletin(identifier=identifier)
+        doc = await self.get_bulletin(identifier=identifier)
         if doc is None:
             # the owner(founder) should be set in the bulletin document of group
             return None
         db = self.archivist
         # check local storage
-        user = db.founder(identifier=identifier)
+        user = await db.get_founder(identifier=identifier)
         if user is not None:
             # got from local storage
             return user
         # get from bulletin document
         user = doc.founder
         if user is None:
             self.error(msg='founder not designated for group: %s' % identifier)
         return user
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
+    async def get_owner(self, identifier: ID) -> Optional[ID]:
         # check broadcast group
         if identifier.is_broadcast:
             # owner of broadcast group
             return BroadcastHelper.broadcast_owner(group=identifier)
         # check bulletin document
-        doc = self.bulletin(identifier=identifier)
+        doc = await self.get_bulletin(identifier=identifier)
         if doc is None:
             # the owner(founder) should be set in the bulletin document of group
             return None
         db = self.archivist
         # check local storage
-        user = db.owner(identifier=identifier)
+        user = await db.get_owner(identifier=identifier)
         if user is not None:
             # got from local storage
             return user
         # check group type
         if identifier.type == EntityType.GROUP:
             # Polylogue's owner is its founder
-            user = db.founder(identifier=identifier)
+            user = await db.get_founder(identifier=identifier)
             if user is None:
                 user = doc.founder
         if user is None:
             self.error(msg='owner not found for group: %s' % identifier)
         return user
 
     # Override
-    def members(self, identifier: ID) -> List[ID]:
-        owner = self.owner(identifier=identifier)
+    async def get_members(self, identifier: ID) -> List[ID]:
+        owner = await self.get_owner(identifier=identifier)
         if owner is None:
             self.error(msg='group empty: %s' % identifier)
             return []
         db = self.archivist
         # check local storage
-        users = db.members(identifier=identifier)
-        db.check_members(group=identifier, members=users)
+        users = await db.get_members(identifier=identifier)
+        await db.check_members(group=identifier, members=users)
         if len(users) == 0:
             users = [owner]
         else:
             assert users[0] == owner, 'group owner must be the first member: %s' % identifier
         return users
 
     # Override
-    def assistants(self, identifier: ID) -> List[ID]:
+    async def get_assistants(self, identifier: ID) -> List[ID]:
         # check bulletin document
-        doc = self.bulletin(identifier=identifier)
+        doc = await self.get_bulletin(identifier=identifier)
         if doc is None:
             # the assistants should be set in the bulletin document of group
             return []
         db = self.archivist
         # check local storage
-        bots = db.assistants(identifier=identifier)
+        bots = await db.get_assistants(identifier=identifier)
         if len(bots) > 0:
             # got from local storage
             return bots
         # get from bulletin document
         bots = doc.assistants
         return [] if bots is None else bots
 
     #
     #   Organizational Structure
     #
 
-    def administrators(self, group: ID) -> List[ID]:
+    async def get_administrators(self, group: ID) -> List[ID]:
         # check bulletin document
-        doc = self.bulletin(identifier=group)
+        doc = await self.get_bulletin(identifier=group)
         if doc is None:
             # the administrators should be set in the bulletin document
             return []
         db = self.archivist
         # the 'administrators' should be saved into local storage
         # when the newest bulletin document received,
         # so we must get them from the local storage only,
         # not from the bulletin document.
-        return db.administrators(group=group)
+        return await db.get_administrators(group=group)
 
     # protected
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
         db = self.archivist
-        return db.save_administrators(administrators, group=group)
+        return await db.save_administrators(administrators, group=group)
 
     # protected
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         db = self.archivist
-        return db.save_members(members, group=group)
+        return await db.save_members(members, group=group)
 
 
 # TODO: ANS?
```

### Comparing `dimples-0.5.8/dimples/client/messenger.py` & `dimples-1.0.0/dimples/client/messenger.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     Transform and send message
 """
 
 from typing import Optional, List
 
 from dimples import EntityType, ID, EVERYONE
+from dimples import Document
 from dimples import Station
 from dimples import Envelope, InstantMessage, ReliableMessage
 from dimples import ContentType, ReceiptCommand, DocumentCommand
 
 from ..common import HandshakeCommand, ReportCommand, LoginCommand
 from ..common import CommonMessenger
 
@@ -48,124 +49,133 @@
 
     @property
     def session(self) -> ClientSession:
         sess = super().session
         assert isinstance(sess, ClientSession), 'session error: %s' % sess
         return sess
 
-    def handshake(self, session_key: Optional[str]):
+    async def handshake(self, session_key: Optional[str]):
         """ send handshake command to current station """
         session = self.session
         station = session.station
         srv_id = station.identifier
         if session_key is None:
             # first handshake
             facebook = self.facebook
             user = facebook.current_user
             assert user is not None, 'current user not found'
-            meta = user.meta
-            visa = user.visa
+            meta = await user.meta
+            visa = await user.visa
             if visa is None:
                 self.warning(msg='user visa not found: %s' % user)
             else:
-                device = {
-                    'os': 'Linux',
-                }
-                visa.set_property(key='sys', value=device)
-                # sign to update
-                pri_key = facebook.private_key_for_visa_signature(identifier=user.identifier)
-                assert pri_key is not None, 'failed to get private key for visa: %s' % visa
-                visa.sign(private_key=pri_key)
+                # clone visa to update
+                doc = Document.parse(document=visa.copy_dictionary())
+                pri_key = await facebook.private_key_for_visa_signature(identifier=user.identifier)
+                if doc is None or pri_key is None:
+                    self.error(msg='should not happen, visa: %s, private key: %s' % (doc, pri_key))
+                else:
+                    # update visa
+                    doc.set_property(key='sys', value={
+                        'os': 'Linux',
+                    })
+                    if doc.sign(private_key=pri_key) is None:
+                        self.error(msg='failed to sign visa: %s, private key: %s' % (doc, pri_key))
+                    elif await facebook.save_document(document=doc):
+                        self.info(msg='visa updated: %s' % doc)
+                        visa = doc
+                    else:
+                        self.error(msg='failed to save visa: %s' % doc)
             env = Envelope.create(sender=user.identifier, receiver=srv_id)
             cmd = HandshakeCommand.start()
             # send first handshake command as broadcast message
             cmd.group = Station.EVERY
             # create instant message with meta & visa
             i_msg = InstantMessage.create(head=env, body=cmd)
             i_msg.set_map(key='meta', value=meta)
             i_msg.set_map(key='visa', value=visa)
-            self.send_instant_message(msg=i_msg, priority=-1)
+            await self.send_instant_message(msg=i_msg, priority=-1)
         else:
             # handshake again
             cmd = HandshakeCommand.restart(session=session_key)
-            self.send_content(sender=None, receiver=srv_id, content=cmd, priority=-1)
+            await self.send_content(sender=None, receiver=srv_id, content=cmd, priority=-1)
 
     # Override
-    def handshake_success(self):
+    async def handshake_success(self):
         # broadcast current documents after handshake success
-        self.broadcast_document()
+        await self.broadcast_document()
 
-    def broadcast_document(self, updated: bool = False):
+    async def broadcast_document(self, updated: bool = False):
         """ broadcast meta & visa document to all stations """
         facebook = self.facebook
         user = facebook.current_user
         assert user is not None, 'current user not found'
         me = user.identifier
-        meta = user.meta
-        visa = user.visa
+        meta = await user.meta
+        visa = await user.visa
         assert visa is not None, 'visa not found: %s' % user
         command = DocumentCommand.response(identifier=me, meta=meta, document=visa)
         archivist = facebook.archivist
         assert isinstance(archivist, ClientArchivist), 'client archivist error: %s' % archivist
         #
         #  send to all contacts
         #
-        contacts = facebook.contacts(identifier=me)
+        contacts = await facebook.get_contacts(identifier=me)
         for item in contacts:
             if archivist.is_documents_respond_expired(identifier=item, force=updated):
                 self.info(msg='sending visa to: %s' % item)
-                self.send_content(sender=me, receiver=item, content=command, priority=1)
+                await self.send_content(sender=me, receiver=item, content=command, priority=1)
             else:
                 # response not expired yet
                 self.debug(msg='document response not expired yet: %s => %s' % (me, item))
         #
         #  broadcast to everyone@everywhere
         #
         if archivist.is_documents_respond_expired(identifier=EVERYONE, force=updated):
             self.info(msg='sending visa to: %s' % EVERYONE)
-            self.send_content(sender=me, receiver=EVERYONE, content=command, priority=1)
+            await self.send_content(sender=me, receiver=EVERYONE, content=command, priority=1)
         else:
             # response not expired yet
             self.debug(msg='document response not expired yet: %s => %s' % (me, EVERYONE))
 
-    def broadcast_login(self, sender: ID, user_agent: str):
+    async def broadcast_login(self, sender: ID, user_agent: str):
         """ send login command to keep roaming """
         # get current station
         station = self.session.station
         assert sender.type != EntityType.STATION, 'station (%s) cannot login: %s' % (sender, station)
         # create login command
         command = LoginCommand(identifier=sender)
         command.agent = user_agent
         command.station = station
         # broadcast to everyone@everywhere
-        self.send_content(sender=sender, receiver=EVERYONE, content=command, priority=1)
+        await self.send_content(sender=sender, receiver=EVERYONE, content=command, priority=1)
 
-    def report_online(self, sender: ID = None):
+    async def report_online(self, sender: ID = None):
         """ send report command to keep user online """
         command = ReportCommand(title=ReportCommand.ONLINE)
-        self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
+        await self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
 
-    def report_offline(self, sender: ID = None):
+    async def report_offline(self, sender: ID = None):
         """ Send report command to let user offline """
         command = ReportCommand(title=ReportCommand.OFFLINE)
-        self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
+        await self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # call super
-        responses = super().process_reliable_message(msg=msg)
+        responses = await super().process_reliable_message(msg=msg)
         if len(responses) == 0 and self._needs_receipt(msg=msg):
             current_user = self.facebook.current_user
             text = 'Message received.'
             res = ReceiptCommand.create(text=text, envelope=msg.envelope)
             env = Envelope.create(sender=current_user.identifier, receiver=msg.sender)
             i_msg = InstantMessage.create(head=env, body=res)
-            s_msg = self.encrypt_message(msg=i_msg)
+            s_msg = await self.encrypt_message(msg=i_msg)
             assert s_msg is not None, 'failed to encrypt message: %s -> %s' % (current_user, msg.sender)
-            r_msg = self.sign_message(msg=s_msg)
+            r_msg = await self.sign_message(msg=s_msg)
             assert r_msg is not None, 'failed to sign message: %s -> %s' % (current_user, msg.sender)
             responses = [r_msg]
         return responses
 
     # noinspection PyMethodMayBeStatic
     def _needs_receipt(self, msg: ReliableMessage) -> bool:
         if msg.type == ContentType.COMMAND:
```

### Comparing `dimples-0.5.8/dimples/client/network/__init__.py` & `dimples-1.0.0/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/network/session.py` & `dimples-1.0.0/dimples/client/network/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,18 @@
 """
 
 import traceback
 from typing import Optional, List
 
 from dimsdk import Station
 
-from startrek.fsm import Delegate as StateDelegate
 from startrek import Docker, DockerStatus
 from startrek import Arrival
 
-from ...utils import Daemon
+from ...utils import Daemon, Runner
 from ...common import SessionDBI
 from ...conn import BaseSession
 from ...conn import MTPStreamArrival
 
 from .state import StateMachine, SessionState
 
 
@@ -95,74 +94,83 @@
         return self.__key
 
     @key.setter
     def key(self, session_key: str):
         self.__key = session_key
 
     @property
+    def fsm(self) -> StateMachine:
+        return self.__fsm
+
+    @property
     def state(self) -> SessionState:
-        ss = self.__fsm.current_state
+        ss = self.fsm.current_state
         assert ss is None or isinstance(ss, SessionState), 'session state error: %s' % ss
         return ss
 
-    def start(self, delegate: StateDelegate):
-        if self.running:
-            self.stop()
-        # start a background thread
+    # Override
+    async def start(self):
+        assert not self.running, 'client session already started: %s' % self
+        # 1. mark this session to running
+        await super().start()
+        # 2. start state machine
+        fsm = self.fsm
+        assert fsm.delegate is not None, 'FSM delegate not set: %s' % self
+        await fsm.start()
+        # 3. start an async task for this session
         self.__daemon.start()
-        # start state machine
-        fsm = self.__fsm
-        fsm.delegate = delegate
-        fsm.start()
 
     # Override
-    def stop(self):
-        super().stop()
-        # stop state machine
-        self.__fsm.stop()
-        # wait for thread stop
+    async def stop(self):
+        # 1. mark this session to stopped
+        await super().stop()
+        # 2. stop state machine
+        await self.fsm.stop()
+        # 3. waiting for the session to stopped
+        await Runner.sleep(seconds=self.interval * 2)
+        # 4. cancel the async task
         self.__daemon.stop()
 
     # Override
-    def setup(self):
+    async def setup(self):
         self.set_active(active=True)
-        super().setup()
+        await super().setup()
 
     # Override
-    def finish(self):
+    async def finish(self):
         self.set_active(active=False)
-        super().finish()
+        await super().finish()
 
     #
     #   Docker Delegate
     #
 
     # Override
-    def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
+    async def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
         # super().docker_status_changed(previous=previous, current=current, docker=docker)
         if current is None or current == DockerStatus.ERROR:
             # connection error or session finished
             self.set_active(active=False)
             self.warning(msg='connection lost, waiting for reconnecting: %s' % docker)
             # TODO: clear session ID and handshake again
         elif current == DockerStatus.READY:
             # connected/reconnected
             self.set_active(active=True)
 
     # Override
-    def docker_received(self, ship: Arrival, docker: Docker):
+    async def docker_received(self, ship: Arrival, docker: Docker):
         # super().docker_received(ship=ship, docker=docker)
         all_responses = []
         messenger = self.messenger
         # 1. get data packages from arrival ship's payload
         packages = get_data_packages(ship=ship)
         for pack in packages:
             try:
                 # 2. process each data package
-                responses = messenger.process_package(data=pack)
+                responses = await messenger.process_package(data=pack)
                 for res in responses:
                     if len(res) == 0:
                         # should not happen
                         continue
                     all_responses.append(res)
             except Exception as error:
                 source = docker.remote_address
@@ -171,15 +179,15 @@
                 # from dimsdk import TextContent
                 # return TextContent.new(text='parse message failed: %s' % error)
         gate = self.gate
         source = docker.remote_address
         destination = docker.local_address
         # 3. send responses separately
         for res in all_responses:
-            gate.send_response(payload=res, ship=ship, remote=source, local=destination)
+            await gate.send_response(payload=res, ship=ship, remote=source, local=destination)
 
 
 def get_data_packages(ship: Arrival) -> List[bytes]:
     assert isinstance(ship, MTPStreamArrival), 'arrival ship error: %s' % ship
     payload = ship.payload
     # check payload
     if payload is None or len(payload) == 0:
```

### Comparing `dimples-0.5.8/dimples/client/network/state.py` & `dimples-1.0.0/dimples/client/network/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,45 +19,61 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
+import asyncio
 import weakref
 from abc import ABC
 from enum import IntEnum
 from typing import Optional, Union
 
 from dimsdk import ID
 
+from startrek.fsm import Runner
 from startrek.fsm import Context, BaseTransition, BaseState, AutoMachine
-from startrek import DockerStatus
+from startrek import Docker, DockerStatus
 
 # from .session import ClientSession
 
 
 class StateMachine(AutoMachine, Context):
 
     def __init__(self, session):
         super().__init__()
         self.__session = weakref.ref(session)
+        self.__docker_ref = None
         # init states
         builder = self._create_state_builder()
         self.add_state(state=builder.get_default_state())
         self.add_state(state=builder.get_connecting_state())
         self.add_state(state=builder.get_connected_state())
         self.add_state(state=builder.get_handshaking_state())
         self.add_state(state=builder.get_running_state())
         self.add_state(state=builder.get_error_state())
 
     @property
     def session(self):  # -> ClientSession:
         return self.__session()
 
+    @property
+    def docker(self) -> Optional[Docker]:
+        ref = self.__docker_ref
+        if ref is not None:
+            return ref()
+
+    @docker.setter
+    def docker(self, worker: Docker):
+        if worker is None:
+            self.__docker_ref = None
+        else:
+            self.__docker_ref = weakref.ref(worker)
+
     # noinspection PyMethodMayBeStatic
     def _create_state_builder(self):
         from .transition import TransitionBuilder
         return StateBuilder(transition_builder=TransitionBuilder())
 
     @property  # Override
     def context(self) -> Context:
@@ -71,21 +87,27 @@
     @property
     def session_id(self) -> ID:
         session = self.session
         return session.identifier
 
     @property
     def status(self) -> DockerStatus:
-        session = self.session
-        gate = session.gate
-        docker = gate.fetch_docker([], remote=session.remote_address, local=None)
-        if docker is None:
-            return DockerStatus.ERROR
-        else:
+        docker = self.docker
+        if docker is not None:
             return docker.status
+        else:
+            session = self.session
+            gate = session.gate
+            task = Runner.async_run(coroutine=gate.fetch_docker([], remote=session.remote_address, local=None))
+            task.add_done_callback(self._fetch_docker_callback)
+        # waiting for callback
+        return DockerStatus.ERROR
+
+    def _fetch_docker_callback(self, t: asyncio.Task):
+        self.docker = t.result()
 
 
 class StateOrder(IntEnum):
     """ Connection State Order """
     INIT = 0  # default
     CONNECTING = 1
     CONNECTED = 2
@@ -171,27 +193,27 @@
             return self.index != other
         elif isinstance(other, str):
             return self.__name != other
         else:
             return True
 
     # Override
-    def on_enter(self, old, ctx: StateMachine, now: float):
+    async def on_enter(self, old, ctx: StateMachine, now: float):
         self.__time = now
 
     # Override
-    def on_exit(self, new, ctx: StateMachine, now: float):
+    async def on_exit(self, new, ctx: StateMachine, now: float):
         self.__time = 0
 
     # Override
-    def on_pause(self, ctx: StateMachine, now: float):
+    async def on_pause(self, ctx: StateMachine, now: float):
         pass
 
     # Override
-    def on_resume(self, ctx: StateMachine, now: float):
+    async def on_resume(self, ctx: StateMachine, now: float):
         pass
 
 
 #
 #   Builders
 #
```

### Comparing `dimples-0.5.8/dimples/client/network/transition.py` & `dimples-1.0.0/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/client/packer.py` & `dimples-1.0.0/dimples/client/packer.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,40 +36,40 @@
 from ..common import CommonMessagePacker
 from .checkpoint import Checkpoint
 
 
 class ClientMessagePacker(CommonMessagePacker):
 
     # Override
-    def _check_receiver(self, msg: InstantMessage) -> bool:
+    async def _check_receiver(self, msg: InstantMessage) -> bool:
         receiver = msg.receiver
         if receiver.is_broadcast:
             # broadcast message
             return True
         elif receiver.is_user:
             # check user's meta & document
-            return super()._check_receiver(msg=msg)
+            return await super()._check_receiver(msg=msg)
         #
         #   check group's meta & members
         #
-        members = self._members(group=receiver)
+        members = await self._members(group=receiver)
         if len(members) == 0:
             # group not ready, suspend message for waiting meta/members
             error = {
                 'message': 'group not ready',
                 'group': str(receiver),
             }
             self.suspend_instant_message(msg=msg, error=error)
             return False
         #
         #   check group members' visa key
         #
         waiting = []
         for item in members:
-            if self._visa_key(user=item) is None:
+            if await self._visa_key(user=item) is None:
                 # member not ready
                 waiting.append(item)
         if len(waiting) == 0:
             # all members' visa keys exist
             return True
         # member(s) not ready, suspend message for waiting document
         error = {
@@ -82,15 +82,15 @@
         # although the packer will query document when the member's visa key is not found,
         # but the station will never respond with the right document,
         # so we must return true here to let the messaging continue;
         # when the member's visa is responded, we should send the suspended message again.
         return len(waiting) < len(members)
 
     # protected
-    def _check_group(self, msg: ReliableMessage) -> bool:
+    async def _check_group(self, msg: ReliableMessage) -> bool:
         receiver = msg.receiver
         # check group
         group = ID.parse(identifier=msg.get('group'))
         if group is None and receiver.is_group:
             # Transform:
             #     (B) => (J)
             #     (D) => (G)
@@ -101,84 +101,84 @@
             #     for this receiver, if no user matched (private key not found),
             #     this message will be ignored;
             # E, F, G - broadcast group message
             #     broadcast message is not encrypted, so it can be read by anyone.
             return True
         # H, J, K - group message
         #     check for received group message
-        members = self._members(group=group)
+        members = await self._members(group=group)
         if len(members) > 0:
             # group is ready
             return True
         # group not ready, suspend message for waiting members
         error = {
             'message': 'group not ready',
             'group': str(receiver),
         }
         self.suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
         return False
 
     # Override
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         # check receiver/group with local user
-        if not self._check_group(msg=msg):
+        if not await self._check_group(msg=msg):
             # receiver (group) not ready
             self.warning(msg='receiver not ready: %s' % msg.receiver)
             return None
-        return super().verify_message(msg=msg)
+        return await super().verify_message(msg=msg)
 
     # # Override
-    # def serialize_message(self, msg: ReliableMessage) -> bytes:
-    #     attach_key_digest(msg=msg, messenger=self.messenger)
-    #     return super().serialize_message(msg=msg)
+    # async def serialize_message(self, msg: ReliableMessage) -> bytes:
+    #     await attach_key_digest(msg=msg, messenger=self.messenger)
+    #     return await super().serialize_message(msg=msg)
 
     # Override
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
-        msg = super().deserialize_message(data=data)
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+        msg = await super().deserialize_message(data=data)
         if msg is not None and self._message_duplicated(msg=msg):
             msg = None
         return msg
 
     def _message_duplicated(self, msg: ReliableMessage) -> bool:
         if g_checkpoint.duplicated(msg=msg):
             sig = get_msg_sig(msg=msg)
             self.warning(msg='drop duplicated message (%s): %s -> %s' % (sig, msg.sender, msg.receiver))
             return True
 
     # # Override
-    # def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+    # async def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
     #     # make sure visa.key exists before encrypting message
-    #     s_msg = super().encrypt_message(msg=msg)
+    #     s_msg = await super().encrypt_message(msg=msg)
     #     receiver = msg.receiver
     #     if receiver.is_group:
     #         # reuse group message keys
-    #         key = self.messenger.cipher_key(sender=msg.sender, receiver=receiver)
+    #         key = await self.messenger.get_cipher_key(sender=msg.sender, receiver=receiver)
     #         key['reused'] = True
     #     # TODO: reuse personal message key?
     #     return s_msg
 
     # # Override
-    # def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
+    # async def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
     #     try:
-    #         return super().decrypt_message(msg=msg)
+    #         await return super().decrypt_message(msg=msg)
     #     except AssertionError as error:
     #         err_msg = '%s' % error
     #         # check exception thrown by DKD: chat.dim.dkd.EncryptedMessage.decrypt()
     #         if err_msg.find('failed to decrypt key in msg') < 0:
     #             raise error
     #         # visa.key expired?
     #         # push new visa document to this message sender
     #         facebook = get_facebook(packer=self)
     #         user = facebook.current_user
     #         current = user.identifier
-    #         visa = user.visa
+    #         visa = await user.visa
     #         assert visa is not None and visa.valid, 'user visa error: %s' % current
     #         command = DocumentCommand.response(document=visa, identifier=current)
     #         messenger = get_messenger(packer=self)
-    #         messenger.send_visa(sender=current, receiver=msg.sender, content=command)
+    #         await messenger.send_visa(sender=current, receiver=msg.sender, content=command)
 
 
 # def get_facebook(packer: CommonMessagePacker) -> CommonFacebook:
 #     barrack = packer.facebook
 #     assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
 #     return barrack
 #
@@ -186,15 +186,15 @@
 # def get_messenger(packer: CommonMessagePacker):
 #     transceiver = packer.messenger
 #     from .messenger import ClientMessenger
 #     assert isinstance(transceiver, ClientMessenger), 'messenger error: %s' % transceiver
 #     return transceiver
 
 
-# def attach_key_digest(msg: ReliableMessage, messenger: Messenger):
+# async def attach_key_digest(msg: ReliableMessage, messenger: Messenger):
 #     # check message delegate
 #     if msg.delegate is None:
 #         msg.delegate = messenger
 #     # check msg.key
 #     if msg.encrypted_key is not None:
 #         # 'key' exists
 #         return
@@ -205,17 +205,17 @@
 #     elif 'digest' in keys:
 #         # key digest already exists
 #         return
 #     # get key with direction
 #     sender = msg.sender
 #     group = msg.group
 #     if group is None:
-#         key = messenger.cipher_key(sender=sender, receiver=msg.receiver)
+#         key = await messenger.get_cipher_key(sender=sender, receiver=msg.receiver)
 #     else:
-#         key = messenger.cipher_key(sender=sender, receiver=group)
+#         key = await messenger.get_cipher_key(sender=sender, receiver=group)
 #     digest = key_digest(key=key)
 #     if digest is None:
 #         # key error
 #         return
 #     keys['digest'] = digest
 #     msg['keys'] = keys
 #
```

### Comparing `dimples-0.5.8/dimples/client/processor.py` & `dimples-1.0.0/dimples/client/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
         assert isinstance(transceiver, CommonMessenger), 'messenger error: %s' % transceiver
         return transceiver
 
     # private
-    def _check_group_times(self, content: Content, r_msg: ReliableMessage) -> bool:
+    async def _check_group_times(self, content: Content, r_msg: ReliableMessage) -> bool:
         group = content.group
         if group is None:
             return False
         facebook = self.facebook
         archivist = facebook.archivist
         assert isinstance(archivist, ClientArchivist), 'client archivist error: %s' % archivist
         now = DateTime.now()
@@ -72,45 +72,45 @@
             if last_doc_time.after(now):
                 # calibrate the clock
                 last_doc_time = now
             doc_updated = archivist.set_last_document_time(identifier=group, last_time=last_doc_time)
             # check whether needs update
             if doc_updated:
                 self.info(msg='checking for new bulletin: %s' % group)
-                facebook.documents(identifier=group)
+                await facebook.get_documents(identifier=group)
         # check group history time
         last_his_time = r_msg.get_datetime(key='GHT', default=None)
         if last_his_time is not None:
             if last_his_time.after(now):
                 # calibrate the clock
                 last_his_time = now
             mem_updated = archivist.set_last_group_history_time(group=group, last_time=last_his_time)
             # check whether needs update
             if mem_updated:
                 archivist.set_last_active_member(member=r_msg.sender, group=group)
                 self.info(msg='checking for group members: %s' % group)
-                facebook.members(identifier=group)
+                await facebook.get_members(identifier=group)
         return doc_updated or mem_updated
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
-        responses = super().process_content(content=content, r_msg=r_msg)
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+        responses = await super().process_content(content=content, r_msg=r_msg)
         # check group document & history times from the message
         # to make sure the group info synchronized
-        self._check_group_times(content=content, r_msg=r_msg)
+        await self._check_group_times(content=content, r_msg=r_msg)
         # check responses
         if len(responses) == 0:
             # respond nothing
             return responses
         elif isinstance(responses[0], HandshakeCommand):
             # urgent command
             return responses
         sender = r_msg.sender
         receiver = r_msg.receiver
-        user = self.facebook.select_user(receiver=receiver)
+        user = await self.facebook.select_user(receiver=receiver)
         if user is None:
             # assert False, 'receiver error: %s' % receiver
             return responses
         receiver = user.identifier
         messenger = self.messenger
         # check responses
         for res in responses:
@@ -126,14 +126,14 @@
             elif isinstance(res, TextContent):
                 if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
                     # no need to respond text message to station
                     when = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(r_msg.time))
                     self.info(msg='drop text responding to %s, origin time=[%s], text=%s' % (sender, when, res.text))
                     continue
             # normal response
-            messenger.send_content(sender=receiver, receiver=sender, content=res)
+            await messenger.send_content(sender=receiver, receiver=sender, content=res)
         # DON'T respond to station directly
         return []
 
     # Override
     def _create_creator(self) -> ContentProcessorCreator:
         return ClientContentProcessorCreator(facebook=self.facebook, messenger=self.messenger)
```

### Comparing `dimples-0.5.8/dimples/client/terminal.py` & `dimples-1.0.0/dimples/client/terminal.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Client
 """
 
 import time
 
 from dimples import EntityType
 
-from ..utils import Runner, Daemon, Logging
+from ..utils import DaemonRunner, Logging
 from ..utils import StateDelegate
 
 from .network import ClientSession
 from .network import StateMachine, SessionState
 from .network.state import StateOrder
 
 from .messenger import ClientMessenger
@@ -47,56 +47,49 @@
 class DeviceMixin:
 
     @property
     def user_agent(self) -> str:
         return 'DIMP/0.4 (Client; Linux; en-US) DIMCoreKit/0.9 (Terminal) DIM-by-GSP/1.0'
 
 
-class Terminal(Runner, DeviceMixin, Logging, StateDelegate):
+class Terminal(DaemonRunner, DeviceMixin, Logging, StateDelegate):
 
     def __init__(self, messenger: ClientMessenger):
         super().__init__(interval=60)
         self.__messenger = messenger
         # default online time
         self.__last_time = time.time()
-        self.__daemon = Daemon(target=self)
 
     @property
     def messenger(self) -> ClientMessenger:
         return self.__messenger
 
     @property
     def session(self) -> ClientSession:
         return self.messenger.session
 
     @property  # Override
     def running(self) -> bool:
         if super().running:
             return self.session.running
 
-    def start(self):
-        self.__daemon.start()
-
-    # Override
-    def stop(self):
-        self.__daemon.stop()
-        super().stop()
-
     # Override
-    def setup(self):
-        super().setup()
-        self.session.start(delegate=self)
+    async def setup(self):
+        await super().setup()
+        session = self.session
+        session.fsm.delegate = self
+        await session.start()
 
     # Override
-    def finish(self):
-        self.session.stop()
-        super().finish()
+    async def finish(self):
+        await self.session.stop()
+        await super().finish()
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         now = time.time()
         if now < (self.__last_time + 300):
             # last sent within 5 minutes
             return False
         # check session state
         messenger = self.messenger
         session = messenger.session
@@ -105,59 +98,59 @@
             # handshake not accepted
             return False
         # report every 5 minutes to keep user online
         if usr_id.type == EntityType.STATION:
             # a station won't login to another station, if here is a station,
             # it must be a station bridge for roaming messages, we just send
             # report command to the target station to keep session online.
-            messenger.report_online(sender=usr_id)
+            await messenger.report_online(sender=usr_id)
         else:
             # send login command to everyone to provide more information.
             # this command can keep the user online too.
-            messenger.broadcast_login(sender=usr_id, user_agent=self.user_agent)
+            await messenger.broadcast_login(sender=usr_id, user_agent=self.user_agent)
         # update last online time
         self.__last_time = now
 
     #
     #   StateDelegate
     #
 
     # Override
-    def enter_state(self, state: SessionState, ctx: StateMachine, now: float):
+    async def enter_state(self, state: SessionState, ctx: StateMachine, now: float):
         # called before state changed
         session = self.session
         station = session.station
         self.info(msg='enter state: %s, %s => %s' % (state, session.identifier, station.identifier))
 
     # Override
-    def exit_state(self, state: SessionState, ctx: StateMachine, now: float):
+    async def exit_state(self, state: SessionState, ctx: StateMachine, now: float):
         # called after state changed
         current = ctx.current_state
         self.info(msg='server state changed: %s -> %s' % (state, current))
         if isinstance(current, SessionState):
             index = current.index
         else:
             index = -1
         if index == StateOrder.HANDSHAKING:
             # start handshake
             messenger = self.messenger
-            messenger.handshake(session_key=None)
+            await messenger.handshake(session_key=None)
         elif index == StateOrder.RUNNING:
             # broadcast current meta & visa document to all stations
             messenger = self.messenger
-            messenger.handshake_success()
+            await messenger.handshake_success()
             session = messenger.session
             usr_id = session.identifier
             if usr_id is not None and usr_id.type != EntityType.STATION:
                 # send login command to everyone to provide more information.
-                messenger.broadcast_login(sender=usr_id, user_agent=self.user_agent)
+                await messenger.broadcast_login(sender=usr_id, user_agent=self.user_agent)
             # update last online time
             self.__last_time = time.time()
 
     # Override
-    def pause_state(self, state: SessionState, ctx: StateMachine, now: float):
+    async def pause_state(self, state: SessionState, ctx: StateMachine, now: float):
         pass
 
     # Override
-    def resume_state(self, state: SessionState, ctx: StateMachine, now: float):
+    async def resume_state(self, state: SessionState, ctx: StateMachine, now: float):
         # TODO: clear session key for re-login?
         pass
```

### Comparing `dimples-0.5.8/dimples/common/__init__.py` & `dimples-1.0.0/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/anonymous.py` & `dimples-1.0.0/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/ans.py` & `dimples-1.0.0/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/archivist.py` & `dimples-1.0.0/dimples/common/archivist.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,141 +74,157 @@
             return ref()
 
     @messenger.setter
     def messenger(self, transceiver: Messenger):
         self.__messenger = weakref.ref(transceiver)
 
     # Override
-    def get_last_group_history_time(self, group: ID) -> Optional[DateTime]:
+    async def get_last_group_history_time(self, group: ID) -> Optional[DateTime]:
         db = self.database
-        array = db.group_histories(group=group)
+        array = await db.get_group_histories(group=group)
         if len(array) == 0:
             return None
         last_time: Optional[DateTime] = None
         for cmd, _ in array:
             his_time = cmd.time
             if his_time is None:
                 assert False, 'group command error: %s' % cmd
                 pass
             elif last_time is None or last_time.before(his_time):
                 last_time = his_time
         return last_time
 
     # # Override
-    # def check_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
+    # async def check_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
     #     if identifier.is_broadcast:
     #         # broadcast entity has no meta to query
     #         return False
     #     return super().check_meta(identifier=identifier, meta=meta)
     #
     # # Override
-    # def check_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    # async def check_documents(self, identifier: ID, documents: List[Document]) -> bool:
     #     if identifier.is_broadcast:
     #         # broadcast entity has no document to update
     #         return False
     #     return super().check_documents(identifier=identifier, documents=documents)
     #
     # # Override
-    # def check_members(self, group: ID, members: List[ID]) -> bool:
+    # async def check_members(self, group: ID, members: List[ID]) -> bool:
     #     if group.is_broadcast:
     #         # broadcast group has no members to update
     #         return False
     #     return super().check_members(group=group, members=members)
 
-    def local_users(self) -> List[ID]:
-        db = self.database
-        return db.local_users()
+    # # Override
+    # async def local_users(self) -> List[ID]:
+    #     db = self.database
+    #     return db.get_local_users()
 
     # Override
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         db = self.database
-        return db.save_meta(meta=meta, identifier=identifier)
+        return await db.save_meta(meta=meta, identifier=identifier)
 
     # Override
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         doc_time = document.time
         if doc_time is None:
             # assert False, 'document error: %s' % doc
             self.warning(msg='document without time: %s' % document.identifier)
         else:
             # calibrate the clock
             # make sure the document time is not in the far future
             current = DateTime.now() + 65.0
             if doc_time > current:
                 # assert False, 'document time error: %s, %s' % (doc_time, document)
                 return False
         db = self.database
-        return db.save_document(document=document)
+        return await db.save_document(document=document)
 
     #
     #   EntityDataSource
     #
 
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    # Override
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         db = self.database
-        return db.meta(identifier=identifier)
+        return await db.get_meta(identifier=identifier)
 
-    def documents(self, identifier: ID) -> List[Document]:
+    # Override
+    async def get_documents(self, identifier: ID) -> List[Document]:
         db = self.database
-        return db.documents(identifier=identifier)
+        return await db.get_documents(identifier=identifier)
 
     #
     #   UserDataSource
     #
 
-    def contacts(self, identifier: ID) -> List[ID]:
+    # Override
+    async def get_contacts(self, identifier: ID) -> List[ID]:
         db = self.database
-        return db.contacts(user=identifier)
+        return await db.get_contacts(user=identifier)
 
-    def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
+    # Override
+    async def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
         raise AssertionError('DON\'T call me!')
 
-    def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
+    # Override
+    async def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
         raise AssertionError('DON\'T call me!')
 
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
+    # Override
+    async def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
         db = self.database
-        return db.private_keys_for_decryption(user=identifier)
+        return await db.private_keys_for_decryption(user=identifier)
 
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
+    # Override
+    async def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.database
-        return db.private_key_for_signature(user=identifier)
+        return await db.private_key_for_signature(user=identifier)
 
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
+    # Override
+    async def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.database
-        return db.private_key_for_visa_signature(user=identifier)
+        return await db.private_key_for_visa_signature(user=identifier)
 
     #
     #   GroupDataSource
     #
 
-    def founder(self, identifier: ID) -> Optional[ID]:
+    # Override
+    async def get_founder(self, identifier: ID) -> Optional[ID]:
         db = self.database
-        return db.founder(group=identifier)
+        return await db.get_founder(group=identifier)
 
-    def owner(self, identifier: ID) -> Optional[ID]:
+    # Override
+    async def get_owner(self, identifier: ID) -> Optional[ID]:
         db = self.database
-        return db.owner(group=identifier)
+        return await db.get_owner(group=identifier)
 
-    def members(self, identifier: ID) -> List[ID]:
+    # Override
+    async def get_members(self, identifier: ID) -> List[ID]:
         db = self.database
-        return db.members(group=identifier)
+        return await db.get_members(group=identifier)
 
-    def assistants(self, identifier: ID) -> List[ID]:
+    # Override
+    async def get_assistants(self, identifier: ID) -> List[ID]:
         db = self.database
-        return db.assistants(group=identifier)
+        return await db.get_assistants(group=identifier)
 
     #
     #   Organization Structure
     #
 
-    def administrators(self, group: ID) -> List[ID]:
+    # Override
+    async def get_administrators(self, group: ID) -> List[ID]:
         db = self.database
-        return db.administrators(group=group)
+        return await db.get_administrators(group=group)
 
-    def save_administrators(self, members: List[ID], group: ID) -> bool:
+    # Override
+    async def save_administrators(self, members: List[ID], group: ID) -> bool:
         db = self.database
-        return db.save_administrators(administrators=members, group=group)
+        return await db.save_administrators(administrators=members, group=group)
 
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    # Override
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         db = self.database
-        return db.save_members(members=members, group=group)
+        return await db.save_members(members=members, group=group)
```

### Comparing `dimples-0.5.8/dimples/common/compat/__init__.py` & `dimples-1.0.0/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/compat/btc.py` & `dimples-1.0.0/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/compat/compatible.py` & `dimples-1.0.0/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/compat/entity.py` & `dimples-1.0.0/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/compat/meta.py` & `dimples-1.0.0/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/compat/network.py` & `dimples-1.0.0/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/dbi/__init__.py` & `dimples-1.0.0/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/dbi/account.py` & `dimples-1.0.0/dimples/common/dbi/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 class PrivateKeyDBI(ABC):
     """ PrivateKey Table """
 
     META = 'M'  # ID_KEY_TAG
     VISA = 'V'  # MSG_KEY_TAG
 
     @abstractmethod
-    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
+    async def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+    async def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
         raise NotImplemented
 
     @abstractmethod
-    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
         raise NotImplemented
 
     @abstractmethod
-    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
         raise NotImplemented
 
     #
     #  Conveniences
     #
 
     @classmethod
@@ -107,144 +107,144 @@
         return -1
 
 
 class MetaDBI(ABC):
     """ Meta Table """
 
     @abstractmethod
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         raise NotImplemented
 
 
 class DocumentDBI(ABC):
     """ Document Table """
 
     @abstractmethod
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def documents(self, identifier: ID) -> List[Document]:
+    async def get_documents(self, identifier: ID) -> List[Document]:
         raise NotImplemented
 
 
 class UserDBI(ABC):
     """ User Table """
 
     @abstractmethod
-    def local_users(self) -> List[ID]:
+    async def get_local_users(self) -> List[ID]:
         """ local user ID list """
         raise NotImplemented
 
     @abstractmethod
-    def save_local_users(self, users: List[ID]) -> bool:
+    async def save_local_users(self, users: List[ID]) -> bool:
         raise NotImplemented
 
 
 class ContactDBI(ABC):
     """ Contact Table """
 
     @abstractmethod
-    def contacts(self, user: ID) -> List[ID]:
+    async def get_contacts(self, user: ID) -> List[ID]:
         """ contacts for user """
         raise NotImplemented
 
     @abstractmethod
-    def save_contacts(self, contacts: List[ID], user: ID) -> bool:
+    async def save_contacts(self, contacts: List[ID], user: ID) -> bool:
         raise NotImplemented
 
 
 class GroupDBI(ABC):
     """ Group/Member Table """
 
     @abstractmethod
-    def founder(self, group: ID) -> Optional[ID]:
+    async def get_founder(self, group: ID) -> Optional[ID]:
         raise NotImplemented
 
     @abstractmethod
-    def owner(self, group: ID) -> Optional[ID]:
+    async def get_owner(self, group: ID) -> Optional[ID]:
         raise NotImplemented
 
     @abstractmethod
-    def members(self, group: ID) -> List[ID]:
+    async def get_members(self, group: ID) -> List[ID]:
         """ group members """
         raise NotImplemented
 
     @abstractmethod
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def assistants(self, group: ID) -> List[ID]:
+    async def get_assistants(self, group: ID) -> List[ID]:
         """ bots for group """
         raise NotImplemented
 
     @abstractmethod
-    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
+    async def save_assistants(self, assistants: List[ID], group: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def administrators(self, group: ID) -> List[ID]:
+    async def get_administrators(self, group: ID) -> List[ID]:
         """ group admins """
         raise NotImplemented
 
     @abstractmethod
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
         raise NotImplemented
 
 
 class GroupHistoryDBI(ABC):
     """ Group History Command Command Table """
 
     @abstractmethod
-    def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
+    async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
         """ save group commands:
                 invite
                 expel (deprecated)
                 join
                 quit
                 reset
                 resign
         """
         raise NotImplemented
 
     @abstractmethod
-    def group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+    async def get_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
         """ load group commands:
                 invite
                 expel (deprecated)
                 join
                 quit
                 reset
                 resign
         """
         raise NotImplemented
 
     @abstractmethod
-    def reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+    async def get_reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
         """ load last 'reset' group command """
         raise NotImplemented
 
     @abstractmethod
-    def clear_group_member_histories(self, group: ID) -> bool:
+    async def clear_group_member_histories(self, group: ID) -> bool:
         """ clear group commands for members:
                 invite
                 expel (deprecated)
                 join
                 quit
                 reset
         """
         raise NotImplemented
 
     @abstractmethod
-    def clear_group_admin_histories(self, group: ID) -> bool:
+    async def clear_group_admin_histories(self, group: ID) -> bool:
         """ clear group commands for administrators:
                 resign
         """
         raise NotImplemented
 
 
 # noinspection PyAbstractClass
```

### Comparing `dimples-0.5.8/dimples/common/dbi/message.py` & `dimples-1.0.0/dimples/common/dbi/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,48 +31,48 @@
 
 class ReliableMessageDBI(ABC):
     """ ReliableMessage Table """
 
     CACHE_LIMIT = 20480  # only cache last messages
 
     @abstractmethod
-    def reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
+    async def get_reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
         """
         Get network messages
 
         :param receiver: actual receiver
         :param limit:    cache limit
         :return: last cached messages
         """
         raise NotImplemented
 
     @abstractmethod
-    def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+    async def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+    async def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         raise NotImplemented
 
 
 # noinspection PyAbstractClass
 class CipherKeyDBI(CipherKeyDelegate, ABC):
     """ CipherKey Table """
     pass
 
 
 class GroupKeysDBI(ABC):
     """ Group Keys Table """
 
     @abstractmethod
-    def group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
+    async def get_group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
         raise NotImplemented
 
     @abstractmethod
-    def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
+    async def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
         raise NotImplemented
 
 
 # noinspection PyAbstractClass
 class MessageDBI(ReliableMessageDBI, CipherKeyDBI, GroupKeysDBI, ABC):
     """ Message Database """
     pass
```

### Comparing `dimples-0.5.8/dimples/common/dbi/session.py` & `dimples-1.0.0/dimples/common/dbi/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 class LoginDBI(ABC):
     """ Login Command Table """
 
     #
     #   login command message
     #
     @abstractmethod
-    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+    async def get_login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
         raise NotImplemented
 
     @abstractmethod
-    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+    async def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         raise NotImplemented
 
 
 #
 #   Service Provider
 #
 
@@ -184,52 +184,52 @@
     general_factory = ProviderGeneralFactory()
 
 
 class ProviderDBI(ABC):
     """ Provider Stations Table """
 
     @abstractmethod
-    def all_providers(self) -> List[ProviderInfo]:
+    async def all_providers(self) -> List[ProviderInfo]:
         """ get list of (SP_ID, chosen) """
         raise NotImplemented
 
     @abstractmethod
-    def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
+    async def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def update_provider(self, identifier: ID, chosen: int) -> bool:
+    async def update_provider(self, identifier: ID, chosen: int) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def remove_provider(self, identifier: ID) -> bool:
+    async def remove_provider(self, identifier: ID) -> bool:
         raise NotImplemented
 
 
 class StationDBI(ABC):
 
     @abstractmethod
-    def all_stations(self, provider: ID) -> List[StationInfo]:
+    async def all_stations(self, provider: ID) -> List[StationInfo]:
         """ get list of (host, port, SP_ID, chosen) """
         raise NotImplemented
 
     @abstractmethod
-    def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
+    async def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = None) -> bool:
+    async def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = None) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def remove_station(self, host: str, port: int, provider: ID) -> bool:
+    async def remove_station(self, host: str, port: int, provider: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    def remove_stations(self, provider: ID) -> bool:
+    async def remove_stations(self, provider: ID) -> bool:
         raise NotImplemented
 
 
 # noinspection PyAbstractClass
 class SessionDBI(LoginDBI, ProviderDBI, StationDBI, ABC):
     """ Session Database """
     pass
```

### Comparing `dimples-0.5.8/dimples/common/facebook.py` & `dimples-1.0.0/dimples/common/facebook.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,176 +64,176 @@
         self.__archivist = db
 
     #
     #   Super
     #
 
     @property  # Override
-    def local_users(self) -> List[User]:
+    async def local_users(self) -> List[User]:
         current = self.__current
         return [] if current is None else [current]
 
     @property
     def current_user(self) -> Optional[User]:
         """ Get current user (for signing and sending message) """
         return self.__current
 
     @current_user.setter
     def current_user(self, user: User):
         if user.data_source is None:
             user.data_source = self
         self.__current = user
 
-    def document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
-        all_documents = self.documents(identifier=identifier)
+    async def get_document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
+        all_documents = await self.get_documents(identifier=identifier)
         doc = DocumentHelper.last_document(all_documents, doc_type)
         # compatible for document type
         if doc is None and doc_type == Document.VISA:
             doc = DocumentHelper.last_document(all_documents, 'profile')
         return doc
 
-    def get_name(self, identifier: ID) -> str:
+    async def get_name(self, identifier: ID) -> str:
         if identifier.is_user:
             doc_type = Document.VISA
         elif identifier.is_group:
             doc_type = Document.BULLETIN
         else:
             doc_type = '*'
         # get name from document
-        doc = self.document(identifier=identifier, doc_type=doc_type)
+        doc = await self.get_document(identifier=identifier, doc_type=doc_type)
         if doc is not None:
             name = doc.name
             if name is not None and len(name) > 0:
                 return name
         # get name from ID
         return Anonymous.get_name(identifier=identifier)
 
     # # Override
-    # def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    # async def save_meta(self, meta: Meta, identifier: ID) -> bool:
     #     # check valid
     #     if meta.valid and meta.match_identifier(identifier=identifier):
     #         pass
     #     else:
     #         # assert False, 'meta not valid: %s' % identifier
     #         return False
     #     # check old meta
-    #     old = self.meta(identifier=identifier)
+    #     old = await self.get_meta(identifier=identifier)
     #     if old is not None:
     #         # assert meta == old, 'meta should not changed'
     #         return True
     #     # meta not exists yet, save it
     #     db = self.database
-    #     return db.save_meta(meta=meta, identifier=identifier)
+    #     return await db.save_meta(meta=meta, identifier=identifier)
     #
     # # Override
-    # def save_document(self, document: Document) -> bool:
+    # async def save_document(self, document: Document) -> bool:
     #     identifier = document.identifier
     #     if not document.valid:
     #         # try to verify
-    #         meta = self.meta(identifier=identifier)
+    #         meta = await self.get_meta(identifier=identifier)
     #         if meta is None:
     #             self.error(msg='meta not found: %s' % identifier)
     #             return False
     #         elif document.verify(public_key=meta.public_key):
     #             self.debug(msg='document verified: %s' % identifier)
     #         else:
     #             self.error(msg='failed to verify document: %s' % identifier)
     #             # assert False, 'document not valid: %s' % identifier
     #             return False
     #     doc_type = document.type
     #     if doc_type is None:
     #         doc_type = '*'
     #     # check old documents with type
-    #     documents = self.documents(identifier=identifier)
+    #     documents = await self.get_documents(identifier=identifier)
     #     old = DocumentHelper.last_document(documents, doc_type)
     #     if old is not None and DocumentHelper.is_expired(document, old):
     #         self.warning(msg='drop expired document: %s' % identifier)
     #         return False
     #     db = self.database
-    #     return db.save_document(document=document)
+    #     return await db.save_document(document=document)
     #
     # #
     # #   EntityDataSource
     # #
     #
     # # Override
-    # def meta(self, identifier: ID) -> Optional[Meta]:
+    # async def get_meta(self, identifier: ID) -> Optional[Meta]:
     #     # if identifier.is_broadcast:
     #     #     # broadcast ID has no meta
     #     #     return None
     #     db = self.database
-    #     return db.meta(identifier=identifier)
+    #     return await db.get_meta(identifier=identifier)
     #
     # # Override
-    # def documents(self, identifier: ID) -> List[Document]:
+    # async def get_documents(self, identifier: ID) -> List[Document]:
     #     # if identifier.is_broadcast:
     #     #     # broadcast ID has no documents
     #     #     return None
     #     db = self.database
-    #     return db.documents(identifier=identifier)
+    #     return await db.get_documents(identifier=identifier)
 
     #
     #   UserDataSource
     #
 
     # Override
-    def contacts(self, identifier: ID) -> List[ID]:
+    async def get_contacts(self, identifier: ID) -> List[ID]:
         db = self.archivist
-        return db.contacts(identifier)
+        return await db.get_contacts(identifier)
 
     # Override
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
+    async def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
         db = self.archivist
-        return db.private_keys_for_decryption(identifier)
+        return await db.private_keys_for_decryption(identifier)
 
     # Override
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
+    async def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.archivist
-        return db.private_key_for_signature(identifier)
+        return await db.private_key_for_signature(identifier)
 
     # Override
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
+    async def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.archivist
-        return db.private_key_for_visa_signature(identifier)
+        return await db.private_key_for_visa_signature(identifier)
 
     # #
     # #    GroupDataSource
     # #
     #
     # # Override
-    # def founder(self, identifier: ID) -> Optional[ID]:
+    # async def get_founder(self, identifier: ID) -> Optional[ID]:
     #     db = self.database
-    #     user = db.founder(group=identifier)
+    #     user = db.get_founder(group=identifier)
     #     if user is None:
-    #         user = super().founder(identifier=identifier)
+    #         user = await super().get_founder(identifier=identifier)
     #     return user
     #
     # # Override
-    # def owner(self, identifier: ID) -> Optional[ID]:
+    # async def get_owner(self, identifier: ID) -> Optional[ID]:
     #     db = self.database
-    #     user = db.owner(group=identifier)
+    #     user = db.get_owner(group=identifier)
     #     if user is None:
-    #         user = super().owner(identifier=identifier)
+    #         user = await super().get_owner(identifier=identifier)
     #     return user
     #
     # # Override
-    # def members(self, identifier: ID) -> List[ID]:
-    #     owner = self.owner(identifier=identifier)
+    # async def get_members(self, identifier: ID) -> List[ID]:
+    #     owner = await self.get_owner(identifier=identifier)
     #     if owner is None:
     #         # assert False, 'group owner not found: %s' % identifier
     #         return []
     #     db = self.database
-    #     users = db.members(group=identifier)
+    #     users = db.get_members(group=identifier)
     #     if len(users) == 0:
-    #         users = super().members(identifier=identifier)
+    #         users = await super().get_members(identifier=identifier)
     #         if len(users) == 0:
     #             users = [owner]
     #     assert owner == users[0], 'group owner must be the first member: %s, group: %s' % (owner, identifier)
     #     return users
     #
     # # Override
-    # def assistants(self, identifier: ID) -> List[ID]:
+    # async def get_assistants(self, identifier: ID) -> List[ID]:
     #     db = self.database
-    #     bots = db.assistants(group=identifier)
+    #     bots = db.get_assistants(group=identifier)
     #     if len(bots) == 0:
-    #         bots = super().assistants(identifier=identifier)
+    #         bots = await super().assistants(identifier=identifier)
     #     return bots
```

### Comparing `dimples-0.5.8/dimples/common/messenger.py` & `dimples-1.0.0/dimples/common/messenger.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,141 +99,143 @@
         return self.__facebook
 
     @property
     def session(self) -> Session:
         return self.__session
 
     @abstractmethod
-    def handshake_success(self):
+    async def handshake_success(self):
         """ callback for handshake success """
         raise NotImplemented
 
     # Override
-    def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
+    async def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
         try:
-            return super().encrypt_key(data=data, receiver=receiver, msg=msg)
+            return await super().encrypt_key(data=data, receiver=receiver, msg=msg)
         except Exception as error:
             # FIXME:
             self.error(msg='failed to encrypt key: %s' % error)
 
     # Override
-    def serialize_key(self, key: Union[dict, SymmetricKey], msg: InstantMessage) -> Optional[bytes]:
+    async def serialize_key(self, key: Union[dict, SymmetricKey], msg: InstantMessage) -> Optional[bytes]:
         # TODO: reuse message key
         #
         # 0. check message key
         reused = key.get('reused')
         digest = key.get('digest')
         if reused is None and digest is None:
             # flags not exist, serialize it directly
-            return super().serialize_key(key=key, msg=msg)
+            return await super().serialize_key(key=key, msg=msg)
         # 1. remove before serializing key
         key.pop('reused', None)
         key.pop('digest', None)
         # 2. serialize key without flags
-        data = super().serialize_key(key=key, msg=msg)
+        data = await super().serialize_key(key=key, msg=msg)
         # 3. put them back after serialized
         if Converter.get_bool(value=reused, default=False):
             key['reused'] = reused
         if digest is not None:
             key['digest'] = digest
         # OK
         return data
 
     # Override
-    def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
+    async def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
         if isinstance(content, Command):
             content = fix_command(content=content)
-        return super().serialize_content(content=content, key=key, msg=msg)
+        return await super().serialize_content(content=content, key=key, msg=msg)
 
     # Override
-    def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
-        content = super().deserialize_content(data=data, key=key, msg=msg)
+    async def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
+        content = await super().deserialize_content(data=data, key=key, msg=msg)
         if isinstance(content, Command):
             content = fix_command(content=content)
         return content
 
     #
     #   Interfaces for Transmitting Message
     #
 
     # Override
-    def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
-                     priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
+    async def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
+                           priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
         """ Send message content with priority """
         if sender is None:
             current = self.facebook.current_user
             assert current is not None, 'current user not set'
             sender = current.identifier
         env = Envelope.create(sender=sender, receiver=receiver)
         i_msg = InstantMessage.create(head=env, body=content)
-        r_msg = self.send_instant_message(msg=i_msg, priority=priority)
+        r_msg = await self.send_instant_message(msg=i_msg, priority=priority)
         return i_msg, r_msg
 
     # private
-    def _attach_visa_time(self, sender: ID, msg: InstantMessage) -> bool:
+    async def _attach_visa_time(self, sender: ID, msg: InstantMessage) -> bool:
         if isinstance(msg.content, DocumentCommand):
             # no need to attach times for command
             return True
-        doc = self.facebook.visa(identifier=sender)
+        doc = await self.facebook.get_visa(identifier=sender)
         if doc is None:
             self.error(msg='failed to get visa document for sender: %s' % sender)
             return False
         # attach sender document time
         last_doc_time = doc.time
         if last_doc_time is None:
             self.error(msg='document error: %s' % doc)
             return False
         else:
             msg.set_datetime(key='SDT', value=last_doc_time)
         return True
 
     # Override
-    def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
+    async def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
         """ send instant message with priority """
         sender = msg.sender
         # 0. check cycled message
         if sender == msg.receiver:
             self.warning(msg='drop cycled message: %s => %s, %s' % (sender, msg.receiver, msg.group))
             # return None
         else:
             self.debug(msg='send instant message message (type=%d): %s => %s, %s'
                            % (msg.content.type, sender, msg.receiver, msg.group))
             # attach sender's document times
             # for the receiver to check whether user info synchronized
-            ok = self._attach_visa_time(sender=sender, msg=msg)
+            ok = await self._attach_visa_time(sender=sender, msg=msg)
             if not ok:
                 self.warning(msg='failed to attach document time: %s => %s' % (sender, msg.content))
         #
         #  1. encrypt message
         #
-        s_msg = self.encrypt_message(msg=msg)
+        s_msg = await self.encrypt_message(msg=msg)
         if s_msg is None:
             # public key not found?
+            self.warning(msg='failed to encrypt message: %s => %s, %s' % (sender, msg.receiver, msg.group))
             return None
         #
         #  2. sign message
         #
-        r_msg = self.sign_message(msg=s_msg)
+        r_msg = await self.sign_message(msg=s_msg)
         if r_msg is None:
             # TODO: set msg.state = error
             raise AssertionError('failed to sign message: %s' % s_msg)
         #
         #  3. send message
         #
-        if self.send_reliable_message(msg=r_msg, priority=priority):
+        if await self.send_reliable_message(msg=r_msg, priority=priority):
             return r_msg
         # failed
+        self.error(msg='failed to send message: %s => %s, %s' % (sender, msg.receiver, msg.group))
 
     # Override
-    def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
+    async def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
         """ send reliable message with priority """
         # # 0. check cycled message
         # if msg.sender == msg.receiver:
         #     self.warning(msg='drop cycled message: %s => %s, %s' % (msg.sender, msg.receiver, msg.group))
         #     return False
         # 1. serialize message
-        data = self.serialize_message(msg=msg)
+        data = await self.serialize_message(msg=msg)
         assert data is not None, 'failed to serialize message: %s' % msg
         # 2. call gate keeper to send the message data package
         #    put message package into the waiting queue of current session
         session = self.session
-        return session.queue_message_package(msg=msg, data=data, priority=priority)
+        return await session.queue_message_package(msg=msg, data=data, priority=priority)
```

### Comparing `dimples-0.5.8/dimples/common/packer.py` & `dimples-1.0.0/dimples/common/packer.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,61 +95,61 @@
             return messages
 
     #
     #   Checking
     #
 
     # protected
-    def _visa_key(self, user: ID) -> Optional[EncryptKey]:
+    async def _visa_key(self, user: ID) -> Optional[EncryptKey]:
         """ for checking whether user's ready """
-        return self.facebook.public_key_for_encryption(identifier=user)
+        return await self.facebook.public_key_for_encryption(identifier=user)
 
     # protected
-    def _members(self, group: ID) -> List[ID]:
+    async def _members(self, group: ID) -> List[ID]:
         """ for checking whether group's ready """
-        return self.facebook.members(identifier=group)
+        return await self.facebook.get_members(identifier=group)
 
     # protected
-    def _check_sender(self, msg: ReliableMessage) -> bool:
+    async def _check_sender(self, msg: ReliableMessage) -> bool:
         """ Check sender before verifying received message """
         sender = msg.sender
         assert sender.is_user, 'sender error: %s' % sender
         # check sender's meta & document
         visa = MessageHelper.get_visa(msg=msg)
         if visa is not None:
             # first handshake?
             assert visa.identifier == sender, 'visa ID not match: %s => %s' % (sender, visa)
             # assert Meta.match_id(meta=msg.meta, identifier=sender), 'meta error: %s' % msg
             return visa.identifier == sender
-        elif self._visa_key(user=sender) is not None:
+        elif await self._visa_key(user=sender) is not None:
             # sender is OK
             return True
         # sender not ready, suspend message for waiting document
         error = {
             'message': 'verify key not found',
             'user': str(sender),
         }
         self.suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
         return False
 
     # protected
-    def _check_receiver(self, msg: InstantMessage) -> bool:
+    async def _check_receiver(self, msg: InstantMessage) -> bool:
         """ Check receiver before encrypting message """
         receiver = msg.receiver
         if receiver.is_broadcast:
             # broadcast message
             return True
         elif receiver.is_group:
             # NOTICE: station will never send group message, so
             #         we don't need to check group info here; and
             #         if a client wants to send group message,
             #         that should be sent to a group bot first,
             #         and the bot will separate it for all members.
             return False
-        elif self._visa_key(user=receiver) is not None:
+        elif await self._visa_key(user=receiver) is not None:
             # receiver is OK
             return True
         # receiver not ready, suspend message for waiting document
         error = {
             'message': 'encrypt key not found',
             'user': str(receiver),
         }
@@ -157,67 +157,67 @@
         return False
 
     #
     #   Packing
     #
 
     # Override
-    def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+    async def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         # 1. check contact info
         # 2. check group members info
-        if not self._check_receiver(msg=msg):
+        if not await self._check_receiver(msg=msg):
             # receiver not ready
             self.warning(msg='receiver not ready: %s' % msg.receiver)
             return None
         content = msg.content
         if isinstance(content, ReceiptCommand):
             # compatible with v1.0
             fix_receipt_command(content=content)
-        return super().encrypt_message(msg=msg)
+        return await super().encrypt_message(msg=msg)
 
     # Override
-    def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
-        i_msg = super().decrypt_message(msg=msg)
+    async def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
+        i_msg = await super().decrypt_message(msg=msg)
         if i_msg is not None:
             content = i_msg.content
             if isinstance(content, ReceiptCommand):
                 # compatible with v1.0
                 fix_receipt_command(content=content)
             elif isinstance(content, DocumentCommand):
                 # compatible with v1.0
                 fix_document_command(content=content)
         return i_msg
 
     # Override
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         # 1. check receiver/group with local user
         # 2. check sender's meta
-        if not self._check_sender(msg=msg):
+        if not await self._check_sender(msg=msg):
             # sender not ready
             self.warning(msg='sender not ready: %s' % msg.sender)
             return None
-        return super().verify_message(msg=msg)
+        return await super().verify_message(msg=msg)
 
     # Override
-    def sign_message(self, msg: SecureMessage) -> ReliableMessage:
+    async def sign_message(self, msg: SecureMessage) -> ReliableMessage:
         if isinstance(msg, ReliableMessage):
             # already signed
             return msg
-        return super().sign_message(msg=msg)
+        return await super().sign_message(msg=msg)
 
     # Override
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         if data is None or len(data) < 2:
             # message data error
             return None
         # elif not (data.startswith(b'{') and data.endswith(b'}')):
         #     # only support JsON format now
         #     return None
-        msg = super().deserialize_message(data=data)
+        msg = await super().deserialize_message(data=data)
         if msg is not None:
             fix_meta_attachment(msg=msg)
         return msg
 
     # Override
-    def serialize_message(self, msg: ReliableMessage) -> bytes:
+    async def serialize_message(self, msg: ReliableMessage) -> bytes:
         fix_meta_attachment(msg=msg)
-        return super().serialize_message(msg=msg)
+        return await super().serialize_message(msg=msg)
```

### Comparing `dimples-0.5.8/dimples/common/processer.py` & `dimples-1.0.0/dimples/common/processer.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 # noinspection PyAbstractClass
 class CommonMessageProcessor(MessageProcessor, Logging, ABC):
 
     # private
     # noinspection PyUnusedLocal
-    def _check_visa_time(self, content: Content, r_msg: ReliableMessage) -> bool:
+    async def _check_visa_time(self, content: Content, r_msg: ReliableMessage) -> bool:
         facebook = self.facebook
         archivist = facebook.archivist
         assert isinstance(archivist, CommonArchivist), 'archivist error: %s' % archivist
         doc_updated = False
         # check sender document time
         last_doc_time = r_msg.get_datetime(key='SDT', default=None)
         if last_doc_time is not None:
@@ -54,17 +54,17 @@
                 # calibrate the clock
                 last_doc_time = now
             sender = r_msg.sender
             doc_updated = archivist.set_last_document_time(identifier=sender, last_time=last_doc_time)
             # check whether needs update
             if doc_updated:
                 self.info(msg='checking for new visa: %s' % sender)
-                facebook.documents(identifier=sender)
+                await facebook.get_documents(identifier=sender)
         return doc_updated
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
-        responses = super().process_content(content=content, r_msg=r_msg)
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+        responses = await super().process_content(content=content, r_msg=r_msg)
         # check sender's document times from the message
         # to make sure the user info synchronized
-        self._check_visa_time(content=content, r_msg=r_msg)
+        await self._check_visa_time(content=content, r_msg=r_msg)
         return responses
```

### Comparing `dimples-0.5.8/dimples/common/protocol/__init__.py` & `dimples-1.0.0/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/ans.py` & `dimples-1.0.0/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/block.py` & `dimples-1.0.0/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/handshake.py` & `dimples-1.0.0/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/login.py` & `dimples-1.0.0/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/mute.py` & `dimples-1.0.0/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/protocol/report.py` & `dimples-1.0.0/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/common/register.py` & `dimples-1.0.0/dimples/common/register.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         super().__init__()
         self.__db = database
 
     @property
     def database(self) -> AccountDBI:
         return self.__db
 
-    def create_user(self, name: str, avatar: Optional[PortableNetworkFile]) -> ID:
+    async def create_user(self, name: str, avatar: Optional[PortableNetworkFile]) -> ID:
         """
         Generate user account
 
         :param name:   user name
         :param avatar: photo URL
         :return: user ID
         """
@@ -78,22 +78,22 @@
         msg_key = PrivateKey.generate(algorithm=AsymmetricKey.RSA)
         visa_key = msg_key.public_key
         visa = self._create_visa(user=identifier, visa_key=visa_key, private_key=id_key, name=name, avatar=avatar)
         #
         #   Step 5: save private key, meta & visa in local storage
         #
         db = self.database
-        db.save_private_key(key=id_key, user=identifier, key_type=PrivateKeyDBI.META)
-        db.save_private_key(key=msg_key, user=identifier, key_type=PrivateKeyDBI.VISA)
-        db.save_meta(meta=meta, identifier=identifier)
-        db.save_document(document=visa)
+        await db.save_private_key(key=id_key, user=identifier, key_type=PrivateKeyDBI.META)
+        await db.save_private_key(key=msg_key, user=identifier, key_type=PrivateKeyDBI.VISA)
+        await db.save_meta(meta=meta, identifier=identifier)
+        await db.save_document(document=visa)
         # OK
         return identifier
 
-    def create_group(self, founder: ID, name: str, seed: str = None) -> ID:
+    async def create_group(self, founder: ID, name: str, seed: str = None) -> ID:
         """
         Generate group account
 
         :param founder: group founder
         :param name:    group title
         :param seed:    ID.name
         :return: group ID
@@ -101,15 +101,15 @@
         if seed is None or len(seed) == 0:
             r = random.randint(10000, 999999999)  # 10,000 ~ 999,999,999
             seed = 'Group-%d' % r
         db = self.database
         #
         #   Step 1: get private key of founder
         #
-        private_key = db.private_key_for_visa_signature(user=founder)
+        private_key = await db.private_key_for_visa_signature(user=founder)
         #
         #   Step 2: generate meta with private key (and meta seed)
         #
         meta = Meta.generate(version=MetaType.MKM, private_key=private_key, seed=seed)
         #
         #   Step 3: generate ID with meta
         #
@@ -117,21 +117,21 @@
         #
         #   Step 4: generate bulletin with ID and sign with founder's private key
         #
         doc = self._create_bulletin(group=identifier, private_key=private_key, name=name, founder=founder)
         #
         #   Step 5: save meta & bulletin in local storage
         #
-        db.save_meta(meta=meta, identifier=identifier)
-        db.save_document(document=doc)
+        await db.save_meta(meta=meta, identifier=identifier)
+        await db.save_document(document=doc)
         #
         #   Step 6: add founder as first member
         #
         members = [founder]
-        db.save_members(members=members, group=identifier)
+        await db.save_members(members=members, group=identifier)
         # OK
         return identifier
 
     # noinspection PyMethodMayBeStatic
     def _create_visa(self, user: ID, visa_key: EncryptKey, private_key: SignKey,
                      name: str, avatar: Optional[PortableNetworkFile]) -> Visa:
         """ create user document """
```

### Comparing `dimples-0.5.8/dimples/common/session.py` & `dimples-1.0.0/dimples/common/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,40 +38,40 @@
 
 from .dbi import SessionDBI
 
 
 class Transmitter(ABC):
 
     @abstractmethod
-    def send_content(self, content: Content, sender: Optional[ID], receiver: ID,
-                     priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
+    async def send_content(self, content: Content, sender: Optional[ID], receiver: ID,
+                           priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
         """
         Send content from sender to receiver with priority
 
         :param content:  message content
         :param sender:   from where
         :param receiver: to where
         :param priority: smaller is faster
         :return: (i_msg, None) on error
         """
         raise NotImplemented
 
     @abstractmethod
-    def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
+    async def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
         """
         Send instant message with priority
 
         :param msg:      plain message
         :param priority: smaller is faster
         :return: None on error
         """
         raise NotImplemented
 
     @abstractmethod
-    def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
+    async def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
         """
         Send reliable message with priority
 
         :param msg:      encrypted & signed message
         :param priority: smaller is faster
         :return: False on error
         """
@@ -120,15 +120,15 @@
         return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
 
     # Override
     def __repr__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
 
-    def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
+    async def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
         """
         Pack message into a waiting queue
 
         :param msg:      network message
         :param data:     serialized message
         :param priority: smaller is faster
         :return: False on error
```

### Comparing `dimples-0.5.8/dimples/conn/__init__.py` & `dimples-1.0.0/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/gate.py` & `dimples-1.0.0/dimples/conn/gate.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import threading
 from abc import ABC
 from typing import Generic, TypeVar, Optional, Union, List
 
 from startrek.types import SocketAddress
 from startrek.net.state import StateOrder
 from startrek import Hub, Channel
-from startrek import Connection, ConnectionState, ActiveConnection
+from startrek import Connection, ConnectionState, BaseConnection, ActiveConnection
 from startrek import Docker, DockerDelegate
 from startrek import Arrival, StarDocker, StarGate
 
 from ..utils import Logging
 
 from .mtp import TransactionID, MTPStreamDocker, MTPHelper
 from .mars import MarsStreamArrival, MarsStreamDocker, MarsHelper
@@ -80,62 +80,63 @@
         return super()._set_docker(docker=docker, remote=remote, local=None)
 
     # Override
     def _remove_docker(self, docker: Optional[Docker],
                        remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Docker]:
         return super()._remove_docker(docker=docker, remote=remote, local=None)
 
-    def fetch_docker(self, advance_party: List[bytes], remote: SocketAddress, local: Optional[SocketAddress]) -> Docker:
+    async def fetch_docker(self, advance_party: List[bytes],
+                           remote: SocketAddress, local: Optional[SocketAddress]) -> Docker:
         # try to get docker
         with self.__lock:
             old = self._get_docker(remote=remote, local=local)
             if old is None:  # and advance_party is not None:
                 # create & cache docker
                 worker = self._create_docker(advance_party, remote=remote, local=local)
                 self._set_docker(worker, remote=remote, local=local)
             else:
                 worker = old
         if old is None:
             hub = self.hub
             assert isinstance(hub, Hub), 'gate hub error: %s' % hub
-            conn = hub.connect(remote=remote, local=local)
+            conn = await hub.connect(remote=remote, local=local)
             if conn is None:
                 # assert False, 'failed to get connection: %s -> %s' % (local, remote)
                 self._remove_docker(worker, remote=remote, local=local)
                 worker = None
             else:
                 assert isinstance(worker, StarDocker), 'docker error: %s, %s' % (remote, worker)
                 # set connection for this docker
-                worker.set_connection(conn)
+                await worker.set_connection(conn)
         return worker
 
-    def send_response(self, payload: bytes, ship: Arrival,
-                      remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
+    async def send_response(self, payload: bytes, ship: Arrival,
+                            remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         worker = self._get_docker(remote=remote, local=local)
         if isinstance(worker, MTPStreamDocker):
             # sn = TransactionID.from_data(data=ship.sn)
             sn = TransactionID.generate()
             pack = MTPHelper.create_message(body=payload, sn=sn)
-            return worker.send_package(pack=pack)
+            return await worker.send_package(pack=pack)
         elif isinstance(worker, MarsStreamDocker):
             assert isinstance(ship, MarsStreamArrival), 'responding ship error: %s' % ship
             mars = MarsHelper.create_respond(head=ship.package.head, payload=payload)
             ship = MarsStreamDocker.create_departure(mars=mars)
-            return worker.send_ship(ship=ship)
+            return await worker.send_ship(ship=ship)
         elif isinstance(worker, WSDocker):
             ship = worker.pack(payload=payload)
-            return worker.send_ship(ship=ship)
+            return await worker.send_ship(ship=ship)
         else:
             raise LookupError('docker error (%s, %s): %s' % (remote, local, worker))
 
     # Override
-    def _heartbeat(self, connection: Connection):
+    async def _heartbeat(self, connection: Connection):
         # let the client to do the job
         if isinstance(connection, ActiveConnection):
-            super()._heartbeat(connection=connection)
+            await super()._heartbeat(connection=connection)
 
     # Override
     def _cache_advance_party(self, data: bytes, connection: Connection) -> List[bytes]:
         # TODO: cache the advance party before decide which docker to use
         if len(data) == 0:
             return []
         else:
@@ -147,51 +148,53 @@
         pass
 
     #
     #   Connection Delegate
     #
 
     # Override
-    def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
-                                 connection: Connection):
+    async def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
+                                       connection: Connection):
         index = -1 if current is None else current.index
         if index == StateOrder.ERROR:
             self.error(msg='connection lost: %s -> %s, %s' % (previous, current, connection.remote_address))
         elif index != StateOrder.EXPIRED and index != StateOrder.MAINTAINING:
             self.debug(msg='connection state changed: %s -> %s, %s' % (previous, current, connection.remote_address))
         try:
-            super().connection_state_changed(previous=previous, current=current, connection=connection)
+            await super().connection_state_changed(previous=previous, current=current, connection=connection)
         except AssertionError as error:
             self.error(msg='connection callback failed: %s' % error)
 
     # Override
-    def connection_received(self, data: bytes, connection: Connection):
+    async def connection_received(self, data: bytes, connection: Connection):
         self.debug(msg='received %d byte(s): %s' % (len(data), connection.remote_address))
-        super().connection_received(data=data, connection=connection)
+        await super().connection_received(data=data, connection=connection)
 
     # Override
-    def connection_sent(self, sent: int, data: bytes, connection: Connection):
-        super().connection_sent(sent=sent, data=data, connection=connection)
+    async def connection_sent(self, sent: int, data: bytes, connection: Connection):
+        await super().connection_sent(sent=sent, data=data, connection=connection)
         self.debug(msg='sent %d byte(s): %s' % (len(data), connection.remote_address))
 
     # Override
-    def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
-        super().connection_failed(error=error, data=data, connection=connection)
+    async def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
+        await super().connection_failed(error=error, data=data, connection=connection)
         self.error(msg='failed to send %d byte(s): %s, remote=%s' % (len(data), error, connection.remote_address))
 
     # Override
-    def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
-        super().connection_error(error=error, connection=connection)
+    async def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
+        await super().connection_error(error=error, connection=connection)
         if error is not None and str(error).startswith('failed to send: '):
             self.warning(msg='ignore socket error: %s, remote=%s' % (error, connection.remote_address))
 
     def get_channel(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
-        hub = self.hub
-        assert isinstance(hub, Hub), 'hub error: %s' % hub
-        return hub.open(remote=remote, local=local)
+        docker = self._get_docker(remote=remote, local=local)
+        if isinstance(docker, StarDocker):
+            conn = docker.connection
+            if isinstance(conn, BaseConnection):
+                return conn.channel
 
 
 #
 #   Server Gates
 #
```

### Comparing `dimples-0.5.8/dimples/conn/gatekeeper.py` & `dimples-1.0.0/dimples/conn/gatekeeper.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from startrek import Docker, DockerStatus, DockerDelegate
 
 from tcp import StreamChannel
 from tcp import ServerHub, ClientHub
 
 from ..utils import get_remote_address, get_local_address
 from ..utils import get_msg_info
-from ..utils import Runner, Logging
+from ..utils import Runner, Log, Logging
 
 from .protocol import DeparturePacker
 
 from .gate import CommonGate, TCPServerGate, TCPClientGate
 from .queue import MessageQueue, MessageWrapper
 
 
@@ -142,14 +142,23 @@
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, max_size)
         print('[SOCKET] send buffer size changed: %d -> %d, %s' % (size, max_size, conn))
         return True
     else:
         print('[SOCKET] send buffer size: %d, %s' % (size, conn))
 
 
+async def _client_connect(hub: Hub, address):
+    conn = await hub.connect(remote=address)
+    if conn is None:
+        Log.error(msg='failed to connect to remote address: %s' % str(address))
+    else:
+        Log.info(msg='connected to remote address: %s, %s' % (address, conn))
+        reset_send_buffer_size(conn=conn)
+
+
 class GateKeeper(Runner, DockerDelegate, Logging):
     """ Keep a gate to remote address """
 
     SEND_BUFFER_SIZE = 64 * 1024  # 64 KB
 
     def __init__(self, remote: Tuple[str, int], sock: Optional[socket.socket]):
         super().__init__(interval=Runner.INTERVAL_SLOW)
@@ -169,25 +178,24 @@
 
     # noinspection PyMethodMayBeStatic
     def _create_hub(self, delegate: ConnectionDelegate, address: Tuple[str, int], sock: Optional[socket.socket]) -> Hub:
         if sock is None:
             # client
             assert address is not None, 'remote address empty'
             hub = StreamClientHub(delegate=delegate)
-            conn = hub.connect(remote=address)
-            reset_send_buffer_size(conn=conn)
-            # TODO: reset send buffer size
+            Runner.async_run(coroutine=_client_connect(hub=hub, address=address))
+            self.info(msg='client hub created: %s' % str(address))
         else:
             # server
             sock.setblocking(False)
             # sock.settimeout(0.5)
             if address is None:
                 address = get_remote_address(sock=sock)
             channel = StreamChannel(remote=address, local=get_local_address(sock=sock))
-            channel.set_socket(sock=sock)
+            Runner.async_run(coroutine=channel.set_socket(sock=sock))
             hub = StreamServerHub(delegate=delegate)
             hub.put_channel(channel=channel)
         return hub
 
     @property
     def remote_address(self) -> Tuple[str, int]:
         return self.__remote
@@ -212,37 +220,37 @@
 
     # @property  # Override
     # def running(self) -> bool:
     #     if super().running:
     #         return self.gate.running
     #
     # # Override
-    # def stop(self):
-    #     super().stop()
-    #     self.gate.stop()
-    #
-    # # Override
-    # def setup(self):
-    #     super().setup()
-    #     self.gate.start()
-    #
-    # # Override
-    # def finish(self):
-    #     self.gate.stop()
-    #     super().finish()
+    # async def stop(self):
+    #     await super().stop()
+    #     await self.gate.stop()
+
+    # Override
+    async def setup(self):
+        # await self.gate.start()
+        pass
+
+    # Override
+    async def finish(self):
+        # await self.gate.stop()
+        pass
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         gate = self.gate
         hub = gate.hub
         # from tcp import Hub
         # assert isinstance(hub, Hub), 'hub error: %s' % hub
         try:
-            incoming = hub.process()
-            outgoing = gate.process()
+            incoming = await hub.process()
+            outgoing = await gate.process()
             if incoming or outgoing:
                 # processed income/outgo packages
                 return True
         except Exception as e:
             self.error(msg='process error: %s' % e)
             traceback.print_exc()
             return False
@@ -259,48 +267,48 @@
         # if msg in this wrapper is None (means sent successfully),
         # it must have been cleaned already, so it should not be empty here.
         msg = wrapper.msg
         if msg is None:
             # msg sent?
             return True
         # try to push
-        ok = gate.send_ship(ship=wrapper, remote=self.remote_address, local=None)
+        ok = await gate.send_ship(ship=wrapper, remote=self.remote_address, local=None)
         if not ok:
             self.error(msg='gate error, failed to send data')
         return ok
 
-    def _docker_pack(self, payload: bytes, priority: int = 0) -> Departure:
-        docker = self.gate.fetch_docker([], remote=self.remote_address, local=None)
+    async def _docker_pack(self, payload: bytes, priority: int = 0) -> Departure:
+        docker = await self.gate.fetch_docker([], remote=self.remote_address, local=None)
         assert isinstance(docker, DeparturePacker), 'departure packer error: %s' % docker
         return docker.pack(payload=payload, priority=priority)
 
     def _queue_append(self, msg: ReliableMessage, ship: Departure) -> bool:
         return self.__queue.append(msg=msg, ship=ship)
 
     #
     #   Docker Delegate
     #
 
     # Override
-    def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
+    async def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
         self.info(msg='docker status changed: %s -> %s, %s' % (previous, current, docker))
 
     # Override
-    def docker_received(self, ship: Arrival, docker: Docker):
+    async def docker_received(self, ship: Arrival, docker: Docker):
         self.debug(msg='docker received a ship: %s, %s' % (ship, docker))
 
     # Override
-    def docker_sent(self, ship: Departure, docker: Docker):
+    async def docker_sent(self, ship: Departure, docker: Docker):
         # TODO: remove sent message from local cache
         pass
 
     # Override
-    def docker_failed(self, error: IOError, ship: Departure, docker: Docker):
+    async def docker_failed(self, error: IOError, ship: Departure, docker: Docker):
         self.error(msg='docker failed to send ship: %s, %s' % (error, docker))
 
     # Override
-    def docker_error(self, error: IOError, ship: Departure, docker: Docker):
+    async def docker_error(self, error: IOError, ship: Departure, docker: Docker):
         self.error(msg='docker error while sending ship: %s, %s' % (error, docker))
         if isinstance(ship, MessageWrapper):
             msg = ship.msg
             if msg is not None:
                 self.error(msg='error message: %s' % get_msg_info(msg=msg))
```

### Comparing `dimples-0.5.8/dimples/conn/mars.py` & `dimples-1.0.0/dimples/conn/mars.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,21 +207,21 @@
                 elif offset < remain_len:
                     data = data[offset:]
                     self.__chunks = data + self.__chunks
                 remain_len -= offset
             return pack, remain_len
 
     # Override
-    def process_received(self, data: bytes):
+    async def process_received(self, data: bytes):
         # the cached data maybe contain sticky packages,
         # so we need to process them circularly here
         self.__package_received = True
         while self.__package_received:
             self.__package_received = False
-            super().process_received(data=data)
+            await super().process_received(data=data)
             data = b''
 
     # Override
     def _get_arrivals(self, data: bytes) -> List[Arrival]:
         ships = []
         while True:
             pack, remain_len = self._parse_package(data=data)
@@ -236,15 +236,15 @@
                 data = b''
             else:
                 # all data processed
                 break
         return ships
 
     # Override
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         assert isinstance(ship, MarsStreamArrival), 'arrival ship error: %s' % ship
         payload = ship.payload
         if payload is None:
             body_len = 0
         else:
             body_len = len(payload)
         mars = ship.package
@@ -261,37 +261,37 @@
             if mars.body is None:
                 # FIXME: should not happen
                 return None
         elif cmd == NetMsgHead.NOOP:
             # handle NOOP request
             if body_len == 0 or payload == NOOP:
                 ship = self.create_departure(mars=mars, priority=DeparturePriority.SLOWER)
-                self.send_ship(ship=ship)
+                await self.send_ship(ship=ship)
                 return None
         # 2. check body
         if body_len == 4:
             if payload == PING:
                 mars = MarsHelper.create_respond(head=head, payload=PONG)
                 ship = self.create_departure(mars=mars, priority=DeparturePriority.SLOWER)
-                self.send_ship(ship=ship)
+                await self.send_ship(ship=ship)
                 return None
             elif payload == PONG:
                 # FIXME: client should not sent 'PONG' to server
                 return None
             elif payload == NOOP:
                 # FIXME: 'NOOP' can only sent by NOOP cmd
                 return None
         # 3. check for response
-        self._check_response(ship=ship)
+        await self._check_response(ship=ship)
         # NOTICE: the delegate must respond mars package with same cmd & seq,
         #         otherwise the connection will be closed by client
         return ship
 
     # Override
-    def heartbeat(self):
+    async def heartbeat(self):
         # heartbeat by client
         pass
 
     # Override
     def pack(self, payload: bytes, priority: int = 0) -> Departure:
         mars = MarsHelper.create_push(payload=payload)
         return self.create_departure(mars=mars, priority=priority)
```

### Comparing `dimples-0.5.8/dimples/conn/mtp.py` & `dimples-1.0.0/dimples/conn/mtp.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,40 +131,40 @@
                 elif offset < data.size:
                     data = data.slice(start=offset)
                     self.__chunks = data.concat(self.__chunks)
                 remain_len -= offset
             return pack
 
     # Override
-    def process_received(self, data: bytes):
+    async def process_received(self, data: bytes):
         # the cached data maybe contain sticky packages,
         # so we need to process them circularly here
         self.__package_received = True
         while self.__package_received:
             self.__package_received = False
-            super().process_received(data=data)
+            await super().process_received(data=data)
             data = b''
 
     # Override
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         assert isinstance(ship, MTPStreamArrival), 'arrival ship error: %s' % ship
         pack = ship.package
         if pack is None:
             fragments = ship.fragments
             count = len(fragments)
             assert count > 0, 'fragments empty: %s' % ship
             pack = fragments[count - 1]
         head = pack.head
         # check body length
         if head.body_length != pack.body.size:
             # sticky data?
             print('[MTP] package not completed: body_len=%d, %s' % (pack.body.size, pack))
             return ship
         # check for response
-        return super()._check_arrival(ship=ship)
+        return await super()._check_arrival(ship=ship)
 
     # Override
     def _create_arrival(self, pack: Package) -> Arrival:
         return MTPStreamArrival(pack=pack)
 
     # Override
     def _create_departure(self, pack: Package, priority: int = 0) -> Departure:
```

### Comparing `dimples-0.5.8/dimples/conn/protocol/__init__.py` & `dimples-1.0.0/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/protocol/mars.py` & `dimples-1.0.0/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/protocol/ws.py` & `dimples-1.0.0/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/queue.py` & `dimples-1.0.0/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/seeker.py` & `dimples-1.0.0/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/conn/session.py` & `dimples-1.0.0/dimples/conn/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,30 +81,30 @@
             return ref()
 
     @messenger.setter
     def messenger(self, transceiver: CommonMessenger):
         self.__messenger = None if transceiver is None else weakref.ref(transceiver)
 
     # Override
-    def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
-        ship = self._docker_pack(payload=data, priority=priority)
+    async def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
+        ship = await self._docker_pack(payload=data, priority=priority)
         return self._queue_append(msg=msg, ship=ship)
 
     #
     #   Transmitter
     #
 
     # Override
-    def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
-                     priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
+    async def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
+                           priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
         messenger = self.messenger
-        return messenger.send_content(sender=sender, receiver=receiver, content=content, priority=priority)
+        return await messenger.send_content(sender=sender, receiver=receiver, content=content, priority=priority)
 
     # Override
-    def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
+    async def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
         messenger = self.messenger
-        return messenger.send_instant_message(msg=msg, priority=priority)
+        return await messenger.send_instant_message(msg=msg, priority=priority)
 
     # Override
-    def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
+    async def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
         messenger = self.messenger
-        return messenger.send_reliable_message(msg=msg, priority=priority)
+        return await messenger.send_reliable_message(msg=msg, priority=priority)
```

### Comparing `dimples-0.5.8/dimples/conn/ws.py` & `dimples-1.0.0/dimples/conn/ws.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # ==============================================================================
 
 import socket
 import threading
 from typing import Optional, List, Tuple
 
 from startrek.types import SocketAddress
+from startrek.fsm import Runner
 from startrek import Arrival, Departure
 from startrek import ArrivalShip, DepartureShip, DeparturePriority
 from startrek import BaseConnection, BaseChannel
 
 from tcp import PlainDocker
 
 from .protocol import WebSocket
@@ -139,35 +140,35 @@
                 data_len = len(data)
                 pack_len = data_len - len(remaining)
                 if pack_len > 0:
                     pack = data[:pack_len]
             return pack, payload, remain_len
 
     # Override
-    def process_received(self, data: bytes):
+    async def process_received(self, data: bytes):
         # the cached data maybe contain sticky packages,
         # so we need to process them circularly here
         self.__package_received = True
         while self.__package_received:
             self.__package_received = False
-            super().process_received(data=data)
+            await super().process_received(data=data)
             data = b''
 
     # Override
     def _get_arrivals(self, data: bytes) -> List[Arrival]:
         # check for first request
         if self.__handshaking:
             # join the data to the memory cache
             data = self.__chunks + data
             self.__chunks = b''
             # parse handshake
             res = WebSocket.handshake(stream=data)
             if res is not None:
                 ship = WSDeparture(package=res, payload=b'')
-                self.send_ship(ship=ship)
+                Runner.async_run(coroutine=self.send_ship(ship=ship))
                 self.__handshaking = False
             elif len(data) < self.MAX_PACK_LENGTH:
                 # waiting for more data
                 self.__chunks = data + self.__chunks
             return []
         # normal state
         ships = []
@@ -182,40 +183,40 @@
                 data = b''
             else:
                 # all data processed
                 break
         return ships
 
     # Override
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         assert isinstance(ship, WSArrival), 'arrival ship error: %s' % ship
         body = ship.payload
         body_len = len(body)
         # 1. check command
         if body_len == 0:
             # data empty
             return None
         elif body_len == 4:
             if body == PING:
                 # 'PING' -> 'PONG'
                 ship = self.pack(payload=PONG, priority=DeparturePriority.SLOWER)
-                self.send_ship(ship=ship)
+                await self.send_ship(ship=ship)
                 return None
             elif body == PONG or body == NOOP:
                 # ignore
                 return None
         elif body == OK:
             # should not happen
             return None
         # NOTICE: the delegate must respond to client in current request,
         #         cause it's a HTTP connection
         return ship
 
     # Override
-    def heartbeat(self):
+    async def heartbeat(self):
         # heartbeat by client
         pass
 
     # Override
     def pack(self, payload: bytes, priority: int = 0) -> Departure:
         req_pack = WebSocket.pack(payload=payload)
         return WSDeparture(package=req_pack, payload=payload, priority=priority)
```

### Comparing `dimples-0.5.8/dimples/database/__init__.py` & `dimples-1.0.0/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/database/account.py` & `dimples-1.0.0/dimples/database/account.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,143 +64,143 @@
         self.__history_table.show_info()
 
     #
     #   PrivateKey DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
-        return self.__private_table.save_private_key(key=key, user=user, key_type=key_type)
+    async def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
+        return await self.__private_table.save_private_key(key=key, user=user, key_type=key_type)
 
     # Override
-    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
-        return self.__private_table.private_keys_for_decryption(user=user)
+    async def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+        return await self.__private_table.private_keys_for_decryption(user=user)
 
     # Override
-    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
-        return self.__private_table.private_key_for_signature(user=user)
+    async def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
+        return await self.__private_table.private_key_for_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
-        return self.__private_table.private_key_for_visa_signature(user=user)
+    async def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+        return await self.__private_table.private_key_for_visa_signature(user=user)
 
     #
     #   Meta DBI
     #
 
     # Override
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         # check meta with ID
         if not meta.match_identifier(identifier=identifier):
             raise ValueError('meta not match: %s => %s' % (identifier, meta))
-        return self.__meta_table.save_meta(meta=meta, identifier=identifier)
+        return await self.__meta_table.save_meta(meta=meta, identifier=identifier)
 
     # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
-        return self.__meta_table.meta(identifier=identifier)
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
+        return await self.__meta_table.get_meta(identifier=identifier)
 
     #
     #   Document DBI
     #
 
     # Override
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         # check meta first
-        meta = self.__meta_table.meta(identifier=document.identifier)
+        meta = await self.__meta_table.get_meta(identifier=document.identifier)
         if meta is None:
             raise LookupError('meta not exists: %s' % document.identifier)
         # check document valid before saving it
         if not (document.valid or document.verify(public_key=meta.public_key)):
             raise ValueError('document error: %s' % document.identifier)
         # check founder in group document
         if isinstance(document, Bulletin):
             founder = document.founder
             if founder is not None:
-                f_meta = self.__meta_table.meta(identifier=founder)
+                f_meta = await self.__meta_table.get_meta(identifier=founder)
                 if f_meta is None or meta.public_key != meta.public_key:
                     raise ValueError('founder error: %s, group: %s' % (founder, document.identifier))
         # document ok, try to save it
-        return self.__doc_table.save_document(document=document)
+        return await self.__doc_table.save_document(document=document)
 
     # Override
-    def documents(self, identifier: ID) -> List[Document]:
-        return self.__doc_table.documents(identifier=identifier)
+    async def get_documents(self, identifier: ID) -> List[Document]:
+        return await self.__doc_table.get_documents(identifier=identifier)
 
     #
     #   User DBI
     #
 
     # Override
-    def local_users(self) -> List[ID]:
-        return self.__user_table.local_users()
+    async def get_local_users(self) -> List[ID]:
+        return await self.__user_table.get_local_users()
 
     # Override
-    def save_local_users(self, users: List[ID]) -> bool:
-        return self.__user_table.save_local_users(users=users)
+    async def save_local_users(self, users: List[ID]) -> bool:
+        return await self.__user_table.save_local_users(users=users)
 
     # Override
-    def contacts(self, user: ID) -> List[ID]:
-        return self.__user_table.contacts(user=user)
+    async def get_contacts(self, user: ID) -> List[ID]:
+        return await self.__user_table.get_contacts(user=user)
 
     # Override
-    def save_contacts(self, contacts: List[ID], user: ID) -> bool:
-        return self.__user_table.save_contacts(contacts=contacts, user=user)
+    async def save_contacts(self, contacts: List[ID], user: ID) -> bool:
+        return await self.__user_table.save_contacts(contacts=contacts, user=user)
 
     #
     #   Group DBI
     #
 
     # Override
-    def founder(self, group: ID) -> Optional[ID]:
-        return self.__group_table.founder(group=group)
+    async def get_founder(self, group: ID) -> Optional[ID]:
+        return await self.__group_table.get_founder(group=group)
 
     # Override
-    def owner(self, group: ID) -> Optional[ID]:
-        return self.__group_table.owner(group=group)
+    async def get_owner(self, group: ID) -> Optional[ID]:
+        return await self.__group_table.get_owner(group=group)
 
     # Override
-    def members(self, group: ID) -> List[ID]:
-        return self.__group_table.members(group=group)
+    async def get_members(self, group: ID) -> List[ID]:
+        return await self.__group_table.get_members(group=group)
 
     # Override
-    def save_members(self, members: List[ID], group: ID) -> bool:
-        return self.__group_table.save_members(members=members, group=group)
+    async def save_members(self, members: List[ID], group: ID) -> bool:
+        return await self.__group_table.save_members(members=members, group=group)
 
     # Override
-    def assistants(self, group: ID) -> List[ID]:
-        return self.__group_table.assistants(group=group)
+    async def get_assistants(self, group: ID) -> List[ID]:
+        return await self.__group_table.get_assistants(group=group)
 
     # Override
-    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
-        return self.__group_table.save_assistants(assistants=assistants, group=group)
+    async def save_assistants(self, assistants: List[ID], group: ID) -> bool:
+        return await self.__group_table.save_assistants(assistants=assistants, group=group)
 
     # Override
-    def administrators(self, group: ID) -> List[ID]:
-        return self.__group_table.administrators(group=group)
+    async def get_administrators(self, group: ID) -> List[ID]:
+        return await self.__group_table.get_administrators(group=group)
 
     # Override
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
-        return self.__group_table.save_administrators(administrators=administrators, group=group)
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+        return await self.__group_table.save_administrators(administrators=administrators, group=group)
 
     #
     #   Group History DBI
     #
 
     # Override
-    def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
-        return self.__history_table.save_group_history(group=group, content=content, message=message)
+    async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
+        return await self.__history_table.save_group_history(group=group, content=content, message=message)
 
     # Override
-    def group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
-        return self.__history_table.group_histories(group=group)
+    async def get_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+        return await self.__history_table.get_group_histories(group=group)
 
     # Override
-    def reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
-        return self.__history_table.reset_command_message(group=group)
+    async def get_reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+        return await self.__history_table.get_reset_command_message(group=group)
 
     # Override
-    def clear_group_member_histories(self, group: ID) -> bool:
-        return self.__history_table.clear_group_member_histories(group=group)
+    async def clear_group_member_histories(self, group: ID) -> bool:
+        return await self.__history_table.clear_group_member_histories(group=group)
 
     # Override
-    def clear_group_admin_histories(self, group: ID) -> bool:
-        return self.__history_table.clear_group_admin_histories(group=group)
+    async def clear_group_admin_histories(self, group: ID) -> bool:
+        return await self.__history_table.clear_group_admin_histories(group=group)
```

### Comparing `dimples-0.5.8/dimples/database/dos/__init__.py` & `dimples-1.0.0/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/database/dos/base.py` & `dimples-1.0.0/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/database/dos/document.py` & `dimples-1.0.0/dimples/database/dos/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,25 @@
         path = self.public_path(self.doc_path)
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
     def __all_path(self, identifier: ID) -> str:
         path = self.public_path(self.all_path)
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
-    def save_documents(self, documents: List[Document], identifier: ID) -> bool:
+    async def save_documents(self, documents: List[Document], identifier: ID) -> bool:
         """ save documents into file """
         path = self.__all_path(identifier=identifier)
         self.info(msg='Saving %d document(s) into: %s' % (len(documents), path))
         array = []
         for doc in documents:
             assert doc.identifier == identifier, 'document ID not matched: %s, %s' % (identifier, doc)
             array.append(doc.dictionary)
         return self.write_json(container=array, path=path)
 
-    def load_documents(self, identifier: ID) -> Optional[List[Document]]:
+    async def load_documents(self, identifier: ID) -> Optional[List[Document]]:
         """ load documents from file """
         path = self.__all_path(identifier=identifier)
         self.info(msg='Loading documents from: %s' % path)
         array = self.read_json(path=path)
         if array is None:
             # file not found
             return None
@@ -78,53 +78,53 @@
             doc = parse_document(dictionary=info, identifier=identifier)
             if info is None:
                 assert False, 'document error: %s, %s' % (identifier, info)
             documents.append(doc)
         self.info(msg='Loaded %d documents from: %s' % (len(documents), path))
         return documents
 
-    def load_document(self, identifier: ID) -> Optional[Document]:
+    async def load_document(self, identifier: ID) -> Optional[Document]:
         """ load document from file """
         path = self.__doc_path(identifier=identifier)
         self.info(msg='Loading document from: %s' % path)
         info = self.read_json(path=path)
         if info is not None:
             return parse_document(dictionary=info, identifier=identifier)
 
     #
     #   Document DBI
     #
 
     # Override
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         """ save document into file """
         identifier = document.identifier
         doc_type = document.type
         # check old documents
-        all_documents = self.documents(identifier=identifier)
+        all_documents = await self.get_documents(identifier=identifier)
         old = DocumentHelper.last_document(all_documents, doc_type)
         if old is None and doc_type == Document.VISA:
             old = DocumentHelper.last_document(all_documents, 'profile')
         if old is not None:
             if DocumentHelper.is_expired(document, old):
                 self.warning(msg='drop expired document: %s' % identifier)
                 return False
             all_documents.remove(old)
         # append it
         all_documents.append(document)
-        return self.save_documents(documents=all_documents, identifier=identifier)
+        return await self.save_documents(documents=all_documents, identifier=identifier)
 
     # Override
-    def documents(self, identifier: ID) -> List[Document]:
+    async def get_documents(self, identifier: ID) -> List[Document]:
         """ load documents from file """
-        all_documents = self.load_documents(identifier=identifier)
+        all_documents = await self.load_documents(identifier=identifier)
         if all_documents is not None:
             return all_documents
         # try old file
-        doc = self.load_document(identifier=identifier)
+        doc = await self.load_document(identifier=identifier)
         return [] if doc is None else [doc]
 
 
 def parse_document(dictionary: dict, identifier: ID = None, doc_type: str = '*') -> Optional[Document]:
     # check document ID
     doc_id = ID.parse(identifier=dictionary.get('ID'))
     assert doc_id is not None, 'document error: %s' % dictionary
```

### Comparing `dimples-0.5.8/dimples/database/dos/group.py` & `dimples-1.0.0/dimples/database/dos/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,67 +68,67 @@
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
     #
     #   Group DBI
     #
 
     # Override
-    def founder(self, group: ID) -> Optional[ID]:
+    async def get_founder(self, group: ID) -> Optional[ID]:
         pass
 
     # Override
-    def owner(self, group: ID) -> Optional[ID]:
+    async def get_owner(self, group: ID) -> Optional[ID]:
         pass
 
     # Override
-    def members(self, group: ID) -> List[ID]:
+    async def get_members(self, group: ID) -> List[ID]:
         """ load members from file """
         path = self.__members_path(identifier=group)
         self.info(msg='Loading members from: %s' % path)
         users = self.read_json(path=path)
         if users is None:
             # members not found
             return []
         return ID.convert(array=users)
 
     # Override
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         """ save members into file """
         path = self.__members_path(identifier=group)
         self.info(msg='Saving members into: %s' % path)
         return self.write_json(container=ID.revert(array=members), path=path)
 
     # Override
-    def assistants(self, group: ID) -> List[ID]:
+    async def get_assistants(self, group: ID) -> List[ID]:
         """ load assistants from file """
         path = self.__assistants_path(identifier=group)
         self.info(msg='Loading assistants from: %s' % path)
         bots = self.read_json(path=path)
         if bots is None:
             # assistants not found
             return []
         return ID.convert(array=bots)
 
     # Override
-    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
+    async def save_assistants(self, assistants: List[ID], group: ID) -> bool:
         """ save assistants into file """
         path = self.__assistants_path(identifier=group)
         self.info(msg='Saving assistants into: %s' % path)
         return self.write_json(container=ID.revert(array=assistants), path=path)
 
     # Override
-    def administrators(self, group: ID) -> List[ID]:
+    async def get_administrators(self, group: ID) -> List[ID]:
         """ load administrators from file """
         path = self.__administrators_path(identifier=group)
         self.info(msg='Loading administrators from: %s' % path)
         users = self.read_json(path=path)
         if users is None:
             # administrators not found
             return []
         return ID.convert(array=users)
 
     # Override
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
         """ save administrators into file """
         path = self.__administrators_path(identifier=group)
         self.info(msg='Saving administrators into: %s' % path)
         return self.write_json(container=ID.revert(array=administrators), path=path)
```

### Comparing `dimples-0.5.8/dimples/database/dos/group_history.py` & `dimples-1.0.0/dimples/database/dos/group_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         path = self.private_path(self.history_path)
         print('!!!  group history path: %s' % path)
 
     def __history_path(self, group: ID) -> str:
         path = self.private_path(self.history_path)
         return template_replace(path, key='ADDRESS', value=str(group.address))
 
-    def load_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+    async def load_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
         path = self.__history_path(group=group)
         self.info(msg='Loading group history from: %s' % path)
         array = self.read_json(path=path)
         if array is None:
             # history not found
             return []
         assert isinstance(array, List), 'group history error: %s, %s' % (array, path)
@@ -71,15 +71,15 @@
             if cmd is None or msg is None:
                 self.error(msg='group history error: %s' % item)
                 continue
             his = (cmd, msg)
             histories.append(his)
         return histories
 
-    def save_group_histories(self, group: ID, histories: List[Tuple[GroupCommand, ReliableMessage]]) -> bool:
+    async def save_group_histories(self, group: ID, histories: List[Tuple[GroupCommand, ReliableMessage]]) -> bool:
         array = []
         for his in histories:
             # assert len(his) == 2, 'group history error: %s' % his
             cmd = his[0]
             msg = his[1]
             item = {
                 'cmd': cmd.dictionary,
@@ -91,67 +91,67 @@
         return self.write_json(container=array, path=path)
 
     #
     #   Group History DBI
     #
 
     # Override
-    def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
-        histories = self.load_group_histories(group=group)
+    async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
+        histories = await self.load_group_histories(group=group)
         item = (content, message)
         histories.append(item)
-        return self.save_group_histories(group=group, histories=histories)
+        return await self.save_group_histories(group=group, histories=histories)
 
     # Override
-    def group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
-        return self.load_group_histories(group=group)
+    async def get_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+        return await self.load_group_histories(group=group)
 
     # Override
-    def reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
-        histories = self.load_group_histories(group=group)
+    async def get_reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+        histories = await self.load_group_histories(group=group)
         pos = len(histories)
         while pos > 0:
             pos -= 1
             his = histories[pos]
             cmd = his[0]
             msg = his[1]
             if isinstance(cmd, ResetCommand):
                 return cmd, msg
         return None, None
 
     # Override
-    def clear_group_member_histories(self, group: ID) -> bool:
-        histories = self.load_group_histories(group=group)
+    async def clear_group_member_histories(self, group: ID) -> bool:
+        histories = await self.load_group_histories(group=group)
         if len(histories) == 0:
             # history empty
             return True
         array = []
         removed = 0
         for his in histories:
             if isinstance(his[0], ResignCommand):
                 # keep 'resign' command messages
                 array.append(his)
             else:
                 # remove other command messages
                 removed += 1
         # if nothing changed, return True
         # else, save new histories
-        return removed == 0 or self.save_group_histories(group=group, histories=array)
+        return removed == 0 or await self.save_group_histories(group=group, histories=array)
 
     # Override
-    def clear_group_admin_histories(self, group: ID) -> bool:
-        histories = self.load_group_histories(group=group)
+    async def clear_group_admin_histories(self, group: ID) -> bool:
+        histories = await self.load_group_histories(group=group)
         if len(histories) == 0:
             # history empty
             return True
         array = []
         removed = 0
         for his in histories:
             if isinstance(his[0], ResignCommand):
                 # remove 'resign' command messages
                 removed += 1
             else:
                 # keep other command messages
                 array.append(his)
         # if nothing changed, return True
         # else, save new histories
-        return removed == 0 or self.save_group_histories(group=group, histories=array)
+        return removed == 0 or await self.save_group_histories(group=group, histories=array)
```

### Comparing `dimples-0.5.8/dimples/database/dos/group_keys.py` & `dimples-1.0.0/dimples/database/dos/group_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
         return template_replace(path, key='GROUP_ADDRESS', value=str(group.address))
 
     #
     #   Group Keys DBI
     #
 
     # Override
-    def group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
+    async def get_group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
         """ load group keys from file """
         path = self.__keys_path(group=group, sender=sender)
         self.info(msg='Loading group keys from: %s' % path)
         return self.read_json(path=path)
 
     # Override
-    def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
+    async def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
         """ save group keys into file """
         path = self.__keys_path(group=group, sender=sender)
         self.info(msg='Saving group keys into: %s' % path)
         return self.write_json(container=keys, path=path)
```

### Comparing `dimples-0.5.8/dimples/database/dos/login.py` & `dimples-1.0.0/dimples/database/dos/login.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,30 +52,30 @@
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
     #
     #   Login DBI
     #
 
     # Override
-    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+    async def get_login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
         """ load login command from file """
         path = self.__login_path(identifier=user)
         self.info(msg='Loading login command from: %s' % path)
         info = self.read_json(path=path)
         if info is None:
             # command not found
             return None, None
         cmd = info.get('cmd')
         msg = info.get('msg')
         if cmd is not None:
             cmd = LoginCommand(content=cmd)
         return cmd, ReliableMessage.parse(msg=msg)
 
     # Override
-    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+    async def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         """ save login command into file """
         info = {
             'cmd': content.dictionary,
             'msg': msg.dictionary
         }
         path = self.__login_path(identifier=user)
         self.info(msg='Saving login command into: %s' % path)
```

### Comparing `dimples-0.5.8/dimples/database/dos/meta.py` & `dimples-1.0.0/dimples/database/dos/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
     #
     #   Meta DBI
     #
 
     # Override
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         """ save meta into file """
         path = self.__meta_path(identifier=identifier)
         self.info(msg='Saving meta into: %s' % path)
         return self.write_json(container=meta.dictionary, path=path)
 
     # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         """ load meta from file """
         path = self.__meta_path(identifier=identifier)
         self.info(msg='Loading meta from: %s' % path)
         info = self.read_json(path=path)
         if info is not None:
             return Meta.parse(meta=info)
```

### Comparing `dimples-0.5.8/dimples/database/dos/private.py` & `dimples-1.0.0/dimples/database/dos/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,33 +103,33 @@
         return keys
 
     #
     #   PrivateKey DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
+    async def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
         if key_type == self.ID_KEY_TAG:
             # save private key for meta
             return self._save_id_key(key=key, identifier=user)
         else:
             # save private key for visa
             return self._save_msg_key(key=key, identifier=user)
 
     # Override
-    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+    async def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
         keys: list = self._load_msg_keys(identifier=user)
         # the 'ID key' could be used for encrypting message too (RSA),
         # so we append it to the decrypt keys here
         id_key = self._load_id_key(identifier=user)
         if isinstance(id_key, DecryptKey) and PrivateKeyDBI.find(item=id_key, array=keys) < 0:
             keys.append(id_key)
         return keys
 
     # Override
-    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
         # TODO: support multi private keys
-        return self.private_key_for_visa_signature(user=user)
+        return await self.private_key_for_visa_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
         return self._load_id_key(identifier=user)
```

### Comparing `dimples-0.5.8/dimples/database/dos/station.py` & `dimples-1.0.0/dimples/database/dos/station.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         return template_replace(path, key='ADDRESS', value=str(provider.address))
 
     #
     #   Provider DBI
     #
 
     # Override
-    def all_providers(self) -> List[ProviderInfo]:
+    async def all_providers(self) -> List[ProviderInfo]:
         """ load providers from file """
         path = self.__providers_path()
         self.info(msg='Loading providers from: %s' % path)
         providers = self.read_json(path=path)
         if providers is None:
             # service providers not found
             return []
@@ -76,28 +76,28 @@
     def _save_providers(self, providers: List[ProviderInfo]) -> bool:
         """ save providers into file """
         path = self.__providers_path()
         self.info(msg='Saving providers into: %s' % path)
         return self.write_json(container=ProviderInfo.revert(array=providers), path=path)
 
     # Override
-    def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
+    async def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
         """ add provider with chosen order """
-        providers = self.all_providers()
+        providers = await self.all_providers()
         for item in providers:
             if item.identifier == identifier:
                 self.warning(msg='provider exists: %s, %s' % (identifier, providers))
                 return True
         providers.insert(0, ProviderInfo(identifier=identifier, chosen=chosen))
         return self._save_providers(providers=providers)
 
     # Override
-    def update_provider(self, identifier: ID, chosen: int) -> bool:
+    async def update_provider(self, identifier: ID, chosen: int) -> bool:
         """ update provider with chosen order """
-        providers = self.all_providers()
+        providers = await self.all_providers()
         info = None
         for item in providers:
             if item.identifier == identifier:
                 if item.chosen == chosen:
                     self.warning(msg='provider not change: %s, %d' % (identifier, chosen))
                     return True
                 info = item
@@ -106,32 +106,32 @@
             info = ProviderInfo(identifier=identifier, chosen=chosen)
             providers.insert(0, info)
         else:
             info.chosen = chosen
         return self._save_providers(providers=providers)
 
     # Override
-    def remove_provider(self, identifier: ID) -> bool:
+    async def remove_provider(self, identifier: ID) -> bool:
         """ remove provider with SP ID """
-        providers = self.all_providers()
+        providers = await self.all_providers()
         info = None
         for item in providers:
             if item.identifier == identifier:
                 info = item
                 break
         if info is not None:
             providers.remove(info)
             return self._save_providers(providers=providers)
 
     #
     #   Station DBI
     #
 
     # Override
-    def all_stations(self, provider: ID) -> List[StationInfo]:
+    async def all_stations(self, provider: ID) -> List[StationInfo]:
         """ load stations with SP ID """
         path = self.__stations_path(provider=provider)
         self.info(msg='Loading stations from: %s' % path)
         stations = self.read_json(path=path)
         if stations is None:
             # stations not found
             return []
@@ -140,28 +140,29 @@
     def _save_stations(self, stations: List[StationInfo], provider: ID) -> bool:
         """ save stations into file """
         path = self.__stations_path(provider=provider)
         self.info(msg='Saving stations into: %s' % path)
         return self.write_json(container=StationInfo.revert(array=stations), path=path)
 
     # Override
-    def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
+    async def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
         """ add station with chosen order """
-        stations = self.all_stations(provider=provider)
+        stations = await self.all_stations(provider=provider)
         for item in stations:
             if item.port == port and item.host == host:
                 self.warning(msg='station exists: %s, %d, %s' % (host, port, stations))
                 return True
         stations.insert(0, StationInfo(identifier=identifier, host=host, port=port, provider=provider, chosen=chosen))
         return self._save_stations(stations=stations, provider=provider)
 
     # Override
-    def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = None) -> bool:
+    async def update_station(self, identifier: Optional[ID], host: str, port: int,
+                             provider: ID, chosen: int = None) -> bool:
         """ update station with SP ID """
-        stations = self.all_stations(provider=provider)
+        stations = await self.all_stations(provider=provider)
         info = None
         for item in stations:
             if item.port == port and item.host == host:
                 if item.chosen == chosen and item.identifier == identifier:
                     self.warning(msg='station not change: %s, %d' % (host, port))
                     return True
                 info = item
@@ -172,27 +173,27 @@
         else:
             if not (identifier is None or identifier.is_broadcast):
                 info.identifier = identifier
             info.chosen = chosen
         return self._save_stations(stations=stations, provider=provider)
 
     # Override
-    def remove_station(self, host: str, port: int, provider: ID) -> bool:
+    async def remove_station(self, host: str, port: int, provider: ID) -> bool:
         """ remove station with SP ID """
-        stations = self.all_stations(provider=provider)
+        stations = await self.all_stations(provider=provider)
         info = None
         for item in stations:
             if item.port == port and item.host == host:
                 info = item
                 break
         if info is not None:
             stations.remove(info)
             return self._save_stations(stations=stations, provider=provider)
 
     # Override
-    def remove_stations(self, provider: ID) -> bool:
+    async def remove_stations(self, provider: ID) -> bool:
         """ remove all stations with SP ID """
-        stations = self.all_stations(provider=provider)
+        stations = await self.all_stations(provider=provider)
         if len(stations) == 0:
             # already empty
             return True
         return self._save_stations(stations=[], provider=provider)
```

### Comparing `dimples-0.5.8/dimples/database/dos/user.py` & `dimples-1.0.0/dimples/database/dos/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,35 +51,35 @@
         return template_replace(path, key='ADDRESS', value=str(identifier.address))
 
     #
     #   User DBI
     #
 
     # Override
-    def local_users(self) -> List[ID]:
+    async def get_local_users(self) -> List[ID]:
         return []
 
     # Override
-    def save_local_users(self, users: List[ID]) -> bool:
+    async def save_local_users(self, users: List[ID]) -> bool:
         pass
 
     #
     #   Contact DBI
     #
 
     # Override
-    def contacts(self, user: ID) -> List[ID]:
+    async def get_contacts(self, user: ID) -> List[ID]:
         """ load contacts from file """
         path = self.__contacts_path(identifier=user)
         self.info(msg='Loading contacts from: %s' % path)
         contacts = self.read_json(path=path)
         if contacts is None:
             # contacts not found
             return []
         return ID.convert(array=contacts)
 
     # Override
-    def save_contacts(self, contacts: List[ID], user: ID) -> bool:
+    async def save_contacts(self, contacts: List[ID], user: ID) -> bool:
         """ save contacts into file """
         path = self.__contacts_path(identifier=user)
         self.info(msg='Saving contacts into: %s' % path)
         return self.write_json(container=ID.revert(array=contacts), path=path)
```

### Comparing `dimples-0.5.8/dimples/database/message.py` & `dimples-1.0.0/dimples/database/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,41 +53,41 @@
         self.__cipher_table.show_info()
         self.__msg_table.show_info()
 
     #
     #   GroupKeys DBI
 
     # Override
-    def group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
-        return self.__group_keys_table.group_keys(group=group, sender=sender)
+    async def get_group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
+        return await self.__group_keys_table.get_group_keys(group=group, sender=sender)
 
     # Override
-    def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
-        return self.__group_keys_table.save_group_keys(group=group, sender=sender, keys=keys)
+    async def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
+        return await self.__group_keys_table.save_group_keys(group=group, sender=sender, keys=keys)
 
     #
     #   CipherKey DBI
     #
 
     # Override
-    def cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
-        return self.__cipher_table.cipher_key(sender=sender, receiver=receiver, generate=generate)
+    async def get_cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
+        return await self.__cipher_table.get_cipher_key(sender=sender, receiver=receiver, generate=generate)
 
     # Override
-    def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
-        return self.__cipher_table.cache_cipher_key(key=key, sender=sender, receiver=receiver)
+    async def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
+        return await self.__cipher_table.cache_cipher_key(key=key, sender=sender, receiver=receiver)
 
     #
     #   ReliableMessage DBI
     #
 
     # Override
-    def reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
-        return self.__msg_table.reliable_messages(receiver=receiver, limit=limit)
+    async def get_reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
+        return await self.__msg_table.get_reliable_messages(receiver=receiver, limit=limit)
 
     # Override
-    def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
-        return self.__msg_table.cache_reliable_message(msg=msg, receiver=receiver)
+    async def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+        return await self.__msg_table.cache_reliable_message(msg=msg, receiver=receiver)
 
     # Override
-    def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
-        return self.__msg_table.remove_reliable_message(msg=msg, receiver=receiver)
+    async def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+        return await self.__msg_table.remove_reliable_message(msg=msg, receiver=receiver)
```

### Comparing `dimples-0.5.8/dimples/database/session.py` & `dimples-1.0.0/dimples/database/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,58 +50,60 @@
         self.__login_table.show_info()
         self.__station_table.show_info()
 
     #
     #   Login DBI
     #
 
-    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
-        return self.__login_table.login_command_message(user=user)
+    async def get_login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+        return await self.__login_table.get_login_command_message(user=user)
 
-    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
-        return self.__login_table.save_login_command_message(user=user, content=content, msg=msg)
+    async def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+        return await self.__login_table.save_login_command_message(user=user, content=content, msg=msg)
 
     #
     #   Provider DBI
     #
 
     # Override
-    def all_providers(self) -> List[ProviderInfo]:
-        return self.__station_table.all_providers()
+    async def all_providers(self) -> List[ProviderInfo]:
+        return await self.__station_table.all_providers()
 
     # Override
-    def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
-        return self.__station_table.add_provider(identifier=identifier, chosen=chosen)
+    async def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
+        return await self.__station_table.add_provider(identifier=identifier, chosen=chosen)
 
     # Override
-    def update_provider(self, identifier: ID, chosen: int) -> bool:
-        return self.__station_table.update_provider(identifier=identifier, chosen=chosen)
+    async def update_provider(self, identifier: ID, chosen: int) -> bool:
+        return await self.__station_table.update_provider(identifier=identifier, chosen=chosen)
 
     # Override
-    def remove_provider(self, identifier: ID) -> bool:
-        return self.__station_table.remove_provider(identifier=identifier)
+    async def remove_provider(self, identifier: ID) -> bool:
+        return await self.__station_table.remove_provider(identifier=identifier)
 
     #
     #   Station DBI
     #
 
     # Override
-    def all_stations(self, provider: ID) -> List[StationInfo]:
-        return self.__station_table.all_stations(provider=provider)
+    async def all_stations(self, provider: ID) -> List[StationInfo]:
+        return await self.__station_table.all_stations(provider=provider)
 
     # Override
-    def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
-        return self.__station_table.add_station(identifier=identifier,
-                                                host=host, port=port, provider=provider, chosen=chosen)
+    async def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID,
+                          chosen: int = 0) -> bool:
+        return await self.__station_table.add_station(identifier=identifier,
+                                                      host=host, port=port, provider=provider, chosen=chosen)
 
     # Override
-    def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
-        return self.__station_table.update_station(identifier=identifier,
-                                                   host=host, port=port, provider=provider, chosen=chosen)
+    async def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID,
+                             chosen: int = 0) -> bool:
+        return await self.__station_table.update_station(identifier=identifier,
+                                                         host=host, port=port, provider=provider, chosen=chosen)
 
     # Override
-    def remove_station(self, host: str, port: int, provider: ID) -> bool:
-        return self.__station_table.remove_station(host=host, port=port, provider=provider)
+    async def remove_station(self, host: str, port: int, provider: ID) -> bool:
+        return await self.__station_table.remove_station(host=host, port=port, provider=provider)
 
     # Override
-    def remove_stations(self, provider: ID) -> bool:
-        return self.__station_table.remove_stations(provider=provider)
+    async def remove_stations(self, provider: ID) -> bool:
+        return await self.__station_table.remove_stations(provider=provider)
```

### Comparing `dimples-0.5.8/dimples/database/t_cipherkey.py` & `dimples-1.0.0/dimples/database/t_cipherkey.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,29 @@
         print('!!!      cipher key in memory only !!!')
 
     #
     #   Cipher Key DBI
     #
 
     # Override
-    def cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
+    async def get_cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
         if receiver.is_broadcast:
             return PlainKey()
         now = DateTime.now()
         direction = (sender, receiver)
         key, _ = self.__keys_cache.fetch(key=direction, now=now)
         if key is None and generate:
             # generate and cache it
             key = SymmetricKey.generate(algorithm=SymmetricKey.AES)
             assert key is not None, 'failed to generate symmetric key'
             self.__keys_cache.update(key=direction, value=key, life_span=self.CACHE_EXPIRES, now=now)
         return key
 
     # Override
-    def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
+    async def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
         if receiver.is_broadcast:
             # no need to store cipher key for broadcast message
             return False
         now = DateTime.now()
         direction = (sender, receiver)
         # 1. store into memory cache
         self.__keys_cache.update(key=direction, value=key, life_span=self.CACHE_EXPIRES, now=now)
```

### Comparing `dimples-0.5.8/dimples/database/t_document.py` & `dimples-1.0.0/dimples/database/t_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,36 +50,36 @@
         self.__dos.show_info()
 
     #
     #   Document DBI
     #
 
     # Override
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         assert document.valid, 'document invalid: %s' % document
         identifier = document.identifier
         doc_type = document.type
         # 0. check old documents
-        all_documents = self.documents(identifier=identifier)
+        all_documents = await self.get_documents(identifier=identifier)
         old = DocumentHelper.last_document(all_documents, doc_type)
         if old is None and doc_type == Document.VISA:
             old = DocumentHelper.last_document(all_documents, 'profile')
         if old is not None:
             if DocumentHelper.is_expired(document, old):
                 # self.warning(msg='drop expired document: %s' % identifier)
                 return False
             all_documents.remove(old)
         all_documents.append(document)
         # 1. store into memory cache
         self.__docs_cache.update(key=identifier, value=all_documents, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_documents(documents=all_documents, identifier=identifier)
+        return await self.__dos.save_documents(documents=all_documents, identifier=identifier)
 
     # Override
-    def documents(self, identifier: ID) -> List[Document]:
+    async def get_documents(self, identifier: ID) -> List[Document]:
         """ get document for ID """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__docs_cache.fetch(key=identifier, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -88,12 +88,12 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.documents(identifier=identifier)
+            value = await self.__dos.get_documents(identifier=identifier)
             # 3. update memory cache
             self.__docs_cache.update(key=identifier, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.5.8/dimples/database/t_group.py` & `dimples-1.0.0/dimples/database/t_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,23 +52,23 @@
         self.__dos.show_info()
 
     #
     #   Group DBI
     #
 
     # Override
-    def founder(self, group: ID) -> Optional[ID]:
+    async def get_founder(self, group: ID) -> Optional[ID]:
         pass
 
     # Override
-    def owner(self, group: ID) -> Optional[ID]:
+    async def get_owner(self, group: ID) -> Optional[ID]:
         pass
 
     # Override
-    def members(self, group: ID) -> List[ID]:
+    async def get_members(self, group: ID) -> List[ID]:
         """ get members of group """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__members_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -77,29 +77,29 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.members(group=group)
+            value = await self.__dos.get_members(group=group)
             # 3. update memory cache
             self.__members_cache.update(key=group, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         # 1. store into memory cache
         self.__members_cache.update(key=group, value=members, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_members(members=members, group=group)
+        return await self.__dos.save_members(members=members, group=group)
 
     # Override
-    def assistants(self, group: ID) -> List[ID]:
+    async def get_assistants(self, group: ID) -> List[ID]:
         """ get assistants of group """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__assistants_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -108,29 +108,29 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.assistants(group=group)
+            value = await self.__dos.get_assistants(group=group)
             # 3. update memory cache
             self.__assistants_cache.update(key=group, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
+    async def save_assistants(self, assistants: List[ID], group: ID) -> bool:
         # 1. store into memory cache
         self.__assistants_cache.update(key=group, value=assistants, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_assistants(assistants=assistants, group=group)
+        return await self.__dos.save_assistants(assistants=assistants, group=group)
 
     # Override
-    def administrators(self, group: ID) -> List[ID]:
+    async def get_administrators(self, group: ID) -> List[ID]:
         """ get administrators of group """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__administrators_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -139,19 +139,19 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.administrators(group=group)
+            value = await self.__dos.get_administrators(group=group)
             # 3. update memory cache
             self.__administrators_cache.update(key=group, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
         # 1. store into memory cache
         self.__administrators_cache.update(key=group, value=administrators, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_administrators(administrators=administrators, group=group)
+        return await self.__dos.save_administrators(administrators=administrators, group=group)
```

### Comparing `dimples-0.5.8/dimples/database/t_group_history.py` & `dimples-1.0.0/dimples/database/t_group_history.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,33 +47,33 @@
         self.__dos = GroupHistoryStorage(root=root, public=public, private=private)
         man = CacheManager()
         self.__history_cache = man.get_pool(name='group.history')  # ID => List
 
     def show_info(self):
         self.__dos.show_info()
 
-    def save_group_histories(self, group: ID, histories: List[Tuple[GroupCommand, ReliableMessage]]) -> bool:
+    async def save_group_histories(self, group: ID, histories: List[Tuple[GroupCommand, ReliableMessage]]) -> bool:
         # 1. store into memory cache
         self.__history_cache.update(key=group, value=histories, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_group_histories(group=group, histories=histories)
+        return await self.__dos.save_group_histories(group=group, histories=histories)
 
     #
     #   Group History DBI
     #
 
     # Override
-    def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
-        histories = self.group_histories(group=group)
+    async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
+        histories = await self.get_group_histories(group=group)
         item = (content, message)
         histories.append(item)
-        return self.save_group_histories(group=group, histories=histories)
+        return await self.save_group_histories(group=group, histories=histories)
 
     # Override
-    def group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+    async def get_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__history_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # cache not load yet, wait to load
@@ -81,38 +81,38 @@
             else:
                 if holder.is_alive(now=now):
                     # data not found
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.group_histories(group=group)
+            value = await self.__dos.get_group_histories(group=group)
             if value is None:
                 value = []  # placeholder
             # 3. update memory cache
             self.__history_cache.update(key=group, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
-        histories = self.group_histories(group=group)
+    async def get_reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+        histories = await self.get_group_histories(group=group)
         pos = len(histories)
         while pos > 0:
             pos -= 1
             his = histories[pos]
             cmd = his[0]
             msg = his[1]
             if isinstance(cmd, ResetCommand):
                 return cmd, msg
         return None, None
 
     # Override
-    def clear_group_member_histories(self, group: ID) -> bool:
-        histories = self.group_histories(group=group)
+    async def clear_group_member_histories(self, group: ID) -> bool:
+        histories = await self.get_group_histories(group=group)
         if len(histories) == 0:
             # history empty
             return True
         array = []
         removed = 0
         for his in histories:
             if isinstance(his[0], ResignCommand):
@@ -122,16 +122,16 @@
                 # remove other command messages
                 removed += 1
         # if nothing changed, return True
         # else, save new histories
         return removed == 0 or self.save_group_histories(group=group, histories=array)
 
     # Override
-    def clear_group_admin_histories(self, group: ID) -> bool:
-        histories = self.group_histories(group=group)
+    async def clear_group_admin_histories(self, group: ID) -> bool:
+        histories = await self.get_group_histories(group=group)
         if len(histories) == 0:
             # history empty
             return True
         array = []
         removed = 0
         for his in histories:
             if isinstance(his[0], ResignCommand):
```

### Comparing `dimples-0.5.8/dimples/database/t_group_keys.py` & `dimples-1.0.0/dimples/database/t_group_keys.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,20 +45,20 @@
         self.__dos = GroupKeysStorage(root=root, public=public, private=private)
         man = CacheManager()
         self.__keys_cache = man.get_pool(name='group.keys')  # (ID, ID) => Dict
 
     def show_info(self):
         self.__dos.show_info()
 
-    def _merge_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> Dict[str, str]:
+    async def _merge_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> Dict[str, str]:
         if 'digest' not in keys:
             # FIXME: old version?
             return keys
         # 0. check old record
-        table = self.group_keys(group=group, sender=sender)
+        table = await self.get_group_keys(group=group, sender=sender)
         if table is None or 'digest' not in table:
             # new keys
             return keys
         elif table.get('digest') != keys.get('digest'):
             # key changed
             return keys
         else:
@@ -69,25 +69,25 @@
             return table
 
     #
     #   Group Keys DBI
     #
 
     # Override
-    def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
+    async def save_group_keys(self, group: ID, sender: ID, keys: Dict[str, str]) -> bool:
         identifier = (group, sender)
         # 0. check old record
-        keys = self._merge_keys(group=group, sender=sender, keys=keys)
+        keys = await self._merge_keys(group=group, sender=sender, keys=keys)
         # 1. store into memory cache
         self.__keys_cache.update(key=identifier, value=keys, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_group_keys(group=group, sender=sender, keys=keys)
+        return await self.__dos.save_group_keys(group=group, sender=sender, keys=keys)
 
     # Override
-    def group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
+    async def get_group_keys(self, group: ID, sender: ID) -> Optional[Dict[str, str]]:
         now = DateTime.now()
         identifier = (group, sender)
         # 1. check memory cache
         value, holder = self.__keys_cache.fetch(key=identifier, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -96,12 +96,12 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return None
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.group_keys(group=group, sender=sender)
+            value = await self.__dos.get_group_keys(group=group, sender=sender)
             # 3. update memory cache
             self.__keys_cache.update(key=identifier, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.5.8/dimples/database/t_login.py` & `dimples-1.0.0/dimples/database/t_login.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,42 +47,42 @@
         self.__dos = LoginStorage(root=root, public=public, private=private)
         man = CacheManager()
         self.__login_cache = man.get_pool(name='login')  # ID => (LoginCommand, ReliableMessage)
 
     def show_info(self):
         self.__dos.show_info()
 
-    def _is_expired(self, user: ID, content: LoginCommand) -> bool:
+    async def _is_expired(self, user: ID, content: LoginCommand) -> bool:
         """ check old record with command time """
         new_time = content.time
         if new_time is None or new_time <= 0:
             return False
         # check old record
-        old, _ = self.login_command_message(user=user)
+        old, _ = await self.get_login_command_message(user=user)
         if old is not None and is_before(old_time=old.time, new_time=new_time):
             # command expired
             return True
 
     #
     #   Login DBI
     #
 
     # Override
-    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+    async def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         # 0. check command time
-        if self._is_expired(user=user, content=content):
+        if await self._is_expired(user=user, content=content):
             # command expired, drop it
             return False
         # 1. store into memory cache
         self.__login_cache.update(key=user, value=(content, msg), life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_login_command_message(user=user, content=content, msg=msg)
+        return await self.__dos.save_login_command_message(user=user, content=content, msg=msg)
 
     # Override
-    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+    async def get_login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
         """ get login command message for user """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__login_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -91,13 +91,13 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return None, None
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            cmd, msg = self.__dos.login_command_message(user=user)
+            cmd, msg = await self.__dos.get_login_command_message(user=user)
             value = (cmd, msg)
             # 3. update memory cache
             self.__login_cache.update(key=user, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.5.8/dimples/database/t_message.py` & `dimples-1.0.0/dimples/database/t_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,27 @@
         print('!!! messages cached in memory only !!!')
 
     #
     #   Reliable Message DBI
     #
 
     # Override
-    def reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
+    async def get_reliable_messages(self, receiver: ID, limit: int = 1024) -> List[ReliableMessage]:
         now = DateTime.now()
         # get all messages
         messages, _ = self.__msg_cache.fetch(key=receiver, now=now)
         if messages is None:
             return []
         # only last cached messages will be returned
         if 0 < limit < len(messages):
             messages = messages[-limit:]
         return messages
 
     # Override
-    def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+    async def cache_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         now = DateTime.now()
         # assert receiver.is_user, 'message receiver error: %s' % receiver
         messages, holder = self.__msg_cache.fetch(key=receiver, now=now)
         if messages is None:
             messages = [msg]
             self.__msg_cache.update(key=receiver, value=messages, life_span=self.CACHE_EXPIRES, now=now)
             return True
@@ -83,15 +83,15 @@
             holder.update(value=messages, now=now)
             return True
         else:
             # duplicated
             return False
 
     # Override
-    def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+    async def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         now = DateTime.now()
         # assert receiver.is_user, 'message receiver error: %s' % receiver
         messages, holder = self.__msg_cache.fetch(key=receiver, now=now)
         if messages is None:
             # not exists
             return False
         index = find_message(msg=msg, messages=messages)
```

### Comparing `dimples-0.5.8/dimples/database/t_meta.py` & `dimples-1.0.0/dimples/database/t_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.__dos.show_info()
 
     #
     #   Meta DBI
     #
 
     # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         """ get meta for ID """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__meta_cache.fetch(key=identifier, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -67,28 +67,28 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return None
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.meta(identifier=identifier)
+            value = await self.__dos.get_meta(identifier=identifier)
             # 3. update memory cache
             if value is None:
                 self.__meta_cache.update(key=identifier, value=value, life_span=300, now=now)
             else:
                 self.__meta_cache.update(key=identifier, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         # assert Meta.match_id(meta=meta, identifier=identifier), 'meta invalid: %s, %s' % (identifier, meta)
         # 0. check old record
-        old = self.meta(identifier=identifier)
+        old = self.get_meta(identifier=identifier)
         if old is not None:
             # meta exists, no need to update it
             return True
         # 1. store into memory cache
         self.__meta_cache.update(key=identifier, value=meta, life_span=36000)
         # 2. store into local storage
-        return self.__dos.save_meta(meta=meta, identifier=identifier)
+        return await self.__dos.save_meta(meta=meta, identifier=identifier)
```

### Comparing `dimples-0.5.8/dimples/database/t_private.py` & `dimples-1.0.0/dimples/database/t_private.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,43 +47,43 @@
         man = CacheManager()
         self.__id_key_cache = man.get_pool(name='private_id_key')      # ID => PrivateKey
         self.__msg_keys_cache = man.get_pool(name='private_msg_keys')  # ID => List[PrivateKey]
 
     def show_info(self):
         self.__dos.show_info()
 
-    def _add_decrypt_key(self, key: PrivateKey, user: ID) -> Optional[List[PrivateKey]]:
-        private_keys = self.private_keys_for_decryption(user=user)
+    async def _add_decrypt_key(self, key: PrivateKey, user: ID) -> Optional[List[PrivateKey]]:
+        private_keys = await self.private_keys_for_decryption(user=user)
         private_keys = PrivateKeyDBI.convert_private_keys(keys=private_keys)
         return PrivateKeyDBI.insert(item=key, array=private_keys)
 
     #
     #   Private Key DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
+    async def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
         now = DateTime.now()
         # 1. update memory cache
         if key_type == PrivateKeyStorage.ID_KEY_TAG:
             # update 'id_key'
             self.__id_key_cache.update(key=user, value=key, life_span=36000, now=now)
         else:
             # add to old keys
             private_keys = self._add_decrypt_key(key=key, user=user)
             if private_keys is None:
                 # key already exists, nothing changed
                 return False
             # update 'msg_keys'
             self.__msg_keys_cache.update(key=user, value=private_keys, life_span=36000, now=now)
         # 2. update local storage
-        return self.__dos.save_private_key(key=key, user=user, key_type=key_type)
+        return await self.__dos.save_private_key(key=key, user=user, key_type=key_type)
 
     # Override
-    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+    async def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
         """ get sign key for ID """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__msg_keys_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -92,30 +92,30 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.private_keys_for_decryption(user=user)
+            value = await self.__dos.private_keys_for_decryption(user=user)
             # 3. update memory cache
             if value is None:
                 self.__msg_keys_cache.update(key=user, value=value, life_span=300, now=now)
             else:
                 self.__msg_keys_cache.update(key=user, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
         # TODO: support multi private keys
-        return self.private_key_for_visa_signature(user=user)
+        return await self.private_key_for_visa_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+    async def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
         """ get sign key for ID """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__id_key_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -124,15 +124,15 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return None
                 # cache expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.private_key_for_visa_signature(user=user)
+            value = await self.__dos.private_key_for_visa_signature(user=user)
             # 3. update memory cache
             if value is None:
                 self.__id_key_cache.update(key=user, value=value, life_span=600, now=now)
             else:
                 self.__id_key_cache.update(key=user, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.5.8/dimples/database/t_station.py` & `dimples-1.0.0/dimples/database/t_station.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.__dos.show_info()
 
     #
     #   Provider DBI
     #
 
     # Override
-    def all_providers(self) -> List[ProviderInfo]:
+    async def all_providers(self) -> List[ProviderInfo]:
         """ get providers """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__dim_cache.fetch(key='providers', now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -70,50 +70,50 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait for reloading
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.all_providers()
+            value = await self.__dos.all_providers()
             if len(value) == 0:
                 # default providers
                 value = [ProviderInfo(identifier=ProviderInfo.GSP, chosen=0)]
             # 3. update memory cache
             self.__dim_cache.update(key='providers', value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
+    async def add_provider(self, identifier: ID, chosen: int = 0) -> bool:
         # 1. clear cache to reload
         self.__dim_cache.erase(key='providers')
         # 2. store into local storage
-        return self.__dos.add_provider(identifier=identifier, chosen=chosen)
+        return await self.__dos.add_provider(identifier=identifier, chosen=chosen)
 
     # Override
-    def update_provider(self, identifier: ID, chosen: int) -> bool:
+    async def update_provider(self, identifier: ID, chosen: int) -> bool:
         # 1. clear cache to reload
         self.__dim_cache.erase(key='providers')
         # 2. store into local storage
-        return self.__dos.update_provider(identifier=identifier, chosen=chosen)
+        return await self.__dos.update_provider(identifier=identifier, chosen=chosen)
 
     # Override
-    def remove_provider(self, identifier: ID) -> bool:
+    async def remove_provider(self, identifier: ID) -> bool:
         # 1. clear cache to reload
         self.__dim_cache.erase(key='providers')
         # 2. store into local storage
-        return self.__dos.remove_provider(identifier=identifier)
+        return await self.__dos.remove_provider(identifier=identifier)
 
     #
     #   Station DBI
     #
 
     # Override
-    def all_stations(self, provider: ID) -> List[StationInfo]:
+    async def all_stations(self, provider: ID) -> List[StationInfo]:
         """ get stations with SP ID """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__stations_cache.fetch(key=provider, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -122,40 +122,44 @@
             else:
                 if holder.is_alive(now=now):
                     # cache not exists
                     return []
                 # cache expired, wait for reloading
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.all_stations(provider=provider)
+            value = await self.__dos.all_stations(provider=provider)
             # 3. update memory cache
             self.__stations_cache.update(key=provider, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
+    async def add_station(self, identifier: Optional[ID], host: str, port: int,
+                          provider: ID, chosen: int = 0) -> bool:
         # 1. clear cache to reload
         self.__stations_cache.erase(key=provider)
         # 2. store into local storage
-        return self.__dos.add_station(identifier=identifier, host=host, port=port, provider=provider, chosen=chosen)
+        return await self.__dos.add_station(identifier=identifier, host=host, port=port,
+                                            provider=provider, chosen=chosen)
 
     # Override
-    def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = None) -> bool:
+    async def update_station(self, identifier: Optional[ID], host: str, port: int,
+                             provider: ID, chosen: int = None) -> bool:
         # 1. clear cache to reload
         self.__stations_cache.erase(key=provider)
         # 2. store into local storage
-        return self.__dos.update_station(identifier=identifier, host=host, port=port, provider=provider, chosen=chosen)
+        return await self.__dos.update_station(identifier=identifier, host=host, port=port,
+                                               provider=provider, chosen=chosen)
 
     # Override
-    def remove_station(self, host: str, port: int, provider: ID) -> bool:
+    async def remove_station(self, host: str, port: int, provider: ID) -> bool:
         # 1. clear cache to reload
         self.__stations_cache.erase(key=provider)
         # 2. store into local storage
-        return self.__dos.remove_station(host=host, port=port, provider=provider)
+        return await self.__dos.remove_station(host=host, port=port, provider=provider)
 
     # Override
-    def remove_stations(self, provider: ID) -> bool:
+    async def remove_stations(self, provider: ID) -> bool:
         # 1. clear cache to reload
         self.__stations_cache.erase(key=provider)
         # 2. store into local storage
-        return self.__dos.remove_stations(provider=provider)
+        return await self.__dos.remove_stations(provider=provider)
```

### Comparing `dimples-0.5.8/dimples/database/t_user.py` & `dimples-1.0.0/dimples/database/t_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 
 from typing import List
 
 from dimsdk import DateTime
 from dimsdk import ID
 
 from ..utils import CacheManager
-from ..common import UserDBI
+from ..common import UserDBI, ContactDBI
 
 from .dos import UserStorage
 
 
-class UserTable(UserDBI):
+class UserTable(UserDBI, ContactDBI):
     """ Implementations of UserDBI """
 
     CACHE_EXPIRES = 300    # seconds
     CACHE_REFRESHING = 32  # seconds
 
     def __init__(self, root: str = None, public: str = None, private: str = None):
         super().__init__()
@@ -50,27 +50,27 @@
         self.__dos.show_info()
 
     #
     #   User DBI
     #
 
     # Override
-    def local_users(self) -> List[ID]:
+    async def get_local_users(self) -> List[ID]:
         return []
 
     # Override
-    def save_local_users(self, users: List[ID]) -> bool:
+    async def save_local_users(self, users: List[ID]) -> bool:
         pass
 
     #
     #   Contact DBI
     #
 
     # Override
-    def contacts(self, user: ID) -> List[ID]:
+    async def get_contacts(self, user: ID) -> List[ID]:
         """ get contacts for user """
         now = DateTime.now()
         # 1. check memory cache
         value, holder = self.__contacts_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
@@ -79,19 +79,19 @@
             else:
                 if holder.is_alive(now=now):
                     # contacts not exists
                     return []
                 # contacts expired, wait to reload
                 holder.renewal(duration=self.CACHE_REFRESHING, now=now)
             # 2. check local storage
-            value = self.__dos.contacts(user=user)
+            value = await self.__dos.get_contacts(user=user)
             # 3. update memory cache
             self.__contacts_cache.update(key=user, value=value, life_span=self.CACHE_EXPIRES, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_contacts(self, contacts: List[ID], user: ID) -> bool:
+    async def save_contacts(self, contacts: List[ID], user: ID) -> bool:
         # 1. store into memory cache
         self.__contacts_cache.update(key=user, value=contacts, life_span=self.CACHE_EXPIRES)
         # 2. store into local storage
-        return self.__dos.save_contacts(contacts=contacts, user=user)
+        return await self.__dos.save_contacts(contacts=contacts, user=user)
```

### Comparing `dimples-0.5.8/dimples/edge/__init__.py` & `dimples-1.0.0/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/edge/octopus.py` & `dimples-1.0.0/dimples/edge/octopus.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from dimsdk import ContentType
 from dimsdk import EntityType, ID
 from dimsdk import ReliableMessage
 from dimsdk import Station
 
 from ..utils import Log, Logging
-from ..utils import Runner, Daemon
+from ..utils import Runner, DaemonRunner
 from ..utils import get_msg_sig
 from ..common import ProviderInfo
 from ..common import MessageDBI, SessionDBI
 from ..common import HandshakeCommand
 
 from ..client import ClientSession
 from ..client import ClientFacebook
@@ -54,24 +54,23 @@
 from ..client import ClientMessageProcessor
 from ..client import Terminal
 
 from .shared import GlobalVariable
 from .shared import create_session
 
 
-class Octopus(Runner, Logging):
+class Octopus(DaemonRunner, Logging):
 
     def __init__(self, shared: GlobalVariable, local_host: str = '127.0.0.1', local_port: int = 9394):
         super().__init__(interval=60)
         self.__shared = shared
         self.__inner = self.create_inner_terminal(host=local_host, port=local_port)
         self.__outers: Set[Terminal] = set()
         self.__outer_map = weakref.WeakValueDictionary()
         self.__outer_lock = threading.Lock()
-        self.__daemon = Daemon(target=self, daemonic=False)
 
     @property
     def shared(self) -> GlobalVariable:
         return self.__shared
 
     @property
     def database(self) -> SessionDBI:
@@ -125,36 +124,36 @@
                     # self.__outers.discard(out)
                     return None
             # create new terminal
             terminal = self.create_outer_terminal(host=host, port=port)
             self.__outers.add(terminal)
             return terminal
 
-    def start(self):
-        self.__daemon.start()
-
     # Override
-    def stop(self):
-        super().stop()
+    async def stop(self):
+        # 1. stop inner terminal
         inner = self.__inner
         if inner is not None:
-            inner.stop()
+            await inner.stop()
+        # 2. stop outer terminals
         with self.__outer_lock:
             outers = set(self.__outers)
         for out in outers:
-            out.stop()
+            await out.stop()
+        # 3. stop runner
+        await super().stop()
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         # get all neighbor stations
         db = self.database
-        providers = db.all_providers()
+        providers = await db.all_providers()
         assert len(providers) > 0, 'service provider not found'
         gsp = providers[0].identifier
-        neighbors = db.all_stations(provider=gsp)
+        neighbors = await db.all_stations(provider=gsp)
         if neighbors is not None:
             neighbors = neighbors.copy()
         # get all outer terminals
         with self.__outer_lock:
             outers = set(self.__outers)
         self.debug(msg='checking %d client(s) with %d neighbor(s)' % (len(outers), len(neighbors)))
         for out in outers:
@@ -184,28 +183,28 @@
         for item in neighbors:
             host = item.host
             port = item.port
             self.debug(msg='connecting neighbor station (%s:%d), client count: %d' % (host, port, len(self.__outers)))
             self.connect(host=host, port=port)
         return False
 
-    def income_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
+    async def income_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
         """ redirect message from remote station """
         sender = msg.sender
         receiver = msg.receiver
         sig = get_msg_sig(msg=msg)
         messenger = self.inner_messenger
-        if messenger.send_reliable_message(msg=msg, priority=priority):
+        if await messenger.send_reliable_message(msg=msg, priority=priority):
             self.info(msg='redirected msg (%s): %s -> %s' % (sig, sender, receiver))
         else:
             self.error(msg='failed to redirect msg (%s): %s -> %s' % (sig, sender, receiver))
         # no need to respond receipt for station
         return []
 
-    def outgo_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
+    async def outgo_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
         """ redirect message to remote station """
         receiver = msg.receiver
         # get neighbor stations
         neighbor = ID.parse(identifier=msg.get('neighbor'))
         if neighbor is not None:
             neighbors = set()
             neighbors.add(neighbor)
@@ -236,15 +235,15 @@
         failed_neighbors = []
         for target in new_recipients:
             messenger = self.get_outer_messenger(identifier=target)
             if messenger is None:
                 # target station not my neighbor
                 self.warning(msg='not my neighbor: %s (%s)' % (target, receiver))
                 failed_neighbors.append(target)
-            elif messenger.send_reliable_message(msg=msg, priority=priority):
+            elif await messenger.send_reliable_message(msg=msg, priority=priority):
                 self.info(msg='redirected msg (%s) to neighbor: %s (%s)' % (sig, target, receiver))
             else:
                 self.error(msg='failed to send to neighbor: %s (%s)' % (target, receiver))
                 failed_neighbors.append(target)
         if len(failed_neighbors) > 0:
             self.error(msg='failed to redirect msg (%s) for receiver (%s): %s' % (sig, receiver, failed_neighbors))
         return []
@@ -263,106 +262,107 @@
         return self.__terminal()
 
     @terminal.setter
     def terminal(self, client: Terminal):
         self.__terminal = weakref.ref(client)
 
     @property
-    def octopus(self):
-        bot = self.__octopus()
+    def octopus(self) -> Optional[Octopus]:
+        ref = self.__octopus
+        bot = None if ref is None else ref()
         assert isinstance(bot, Octopus), 'octopus error: %s' % bot
         return bot
 
     @octopus.setter
-    def octopus(self, bot):
+    def octopus(self, bot: Octopus):
         self.__octopus = weakref.ref(bot)
 
     @property
     def local_station(self) -> ID:
         facebook = self.facebook
         current = facebook.current_user
         return current.identifier
 
-    def __is_handshaking(self, msg: ReliableMessage) -> bool:
+    async def __is_handshaking(self, msg: ReliableMessage) -> bool:
         """ check HandshakeCommand sent to this station """
         receiver = msg.receiver
         if receiver.type != EntityType.STATION or receiver != self.local_station:
             # not for this station
             return False
         if msg.type != ContentType.COMMAND:
             # not a command
             return False
-        i_msg = self.decrypt_message(msg=msg)
+        i_msg = await self.decrypt_message(msg=msg)
         if i_msg is not None:
             return isinstance(i_msg.content, HandshakeCommand)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # check for HandshakeCommand
-        if self.__is_handshaking(msg=msg):
+        if await self.__is_handshaking(msg=msg):
             self.info(msg='receive handshaking: %s' % msg.sender)
-            return super().process_reliable_message(msg=msg)
+            return await super().process_reliable_message(msg=msg)
         # check for cycled message
         if msg.receiver == msg.sender:
             self.error(msg='drop cycled msg(type=%d): %s -> %s | from %s, traces: %s'
                        % (msg.type, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
             return []
         # handshake accepted, redirecting message
         sig = get_msg_sig(msg=msg)
         self.info(msg='redirect msg(type=%d, sig=%s): %s -> %s | from %s, traces: %s'
                   % (msg.type, sig, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
-        return self._deliver_message(msg=msg)
+        return await self._deliver_message(msg=msg)
 
     @abstractmethod
-    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         """ call octopus to redirect message """
         return []
 
 
 def get_remote_station(messenger: ClientMessenger) -> ID:
     session = messenger.session
     station = session.station
     return station.identifier
 
 
 class InnerMessenger(OctopusMessenger):
     """ Messenger for local station """
 
     # Override
-    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         priority = 0  # NORMAL
         if msg.receiver.is_broadcast:
             priority = 1  # SLOWER
         octopus = self.octopus
-        return octopus.outgo_message(msg=msg, priority=priority)
+        return await octopus.outgo_message(msg=msg, priority=priority)
 
 
 class OuterMessenger(OctopusMessenger):
     """ Messenger for remote station """
 
     # Override
-    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         priority = 0  # NORMAL
         if msg.receiver.is_broadcast:
             priority = 1  # SLOWER
         octopus = self.octopus
-        return octopus.income_message(msg=msg, priority=priority)
+        return await octopus.income_message(msg=msg, priority=priority)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         if msg.sender == self.local_station:
-            self.debug(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
+            self.error(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
             return []
-        return super().process_reliable_message(msg=msg)
+        return await super().process_reliable_message(msg=msg)
 
     # Override
-    def handshake_success(self):
-        super().handshake_success()
+    async def handshake_success(self):
+        await super().handshake_success()
         station = self.session.station
-        update_station(station=station, database=self.octopus.database)
+        await update_station(station=station, database=self.octopus.database)
         octopus = self.octopus
         octopus.add_index(identifier=station.identifier, terminal=self.terminal)
 
 
 def create_messenger(facebook: ClientFacebook, database: MessageDBI,
                      session: ClientSession, messenger_class) -> OctopusMessenger:
     assert issubclass(messenger_class, OctopusMessenger), 'messenger class error: %s' % messenger_class
@@ -376,24 +376,24 @@
     session.messenger = messenger
     return messenger
 
 
 def create_terminal(messenger: OctopusMessenger) -> Terminal:
     terminal = Terminal(messenger=messenger)
     messenger.terminal = terminal
-    terminal.start()
+    Runner.async_run(coroutine=terminal.start())
     return terminal
 
 
-def update_station(station: Station, database: SessionDBI):
+async def update_station(station: Station, database: SessionDBI):
     Log.info(msg='update station: %s' % station)
     # SP ID
     provider = station.provider
     if provider is None:
         provider = ProviderInfo.GSP
     # new info
     sid = station.identifier
     host = station.host
     port = station.port
     assert not sid.is_broadcast, 'station ID error: %s' % sid
     assert host is not None and port > 0, 'station error: %s, %d' % (host, port)
-    database.update_station(identifier=sid, host=host, port=port, provider=provider, chosen=0)
+    await database.update_station(identifier=sid, host=host, port=port, provider=provider, chosen=0)
```

### Comparing `dimples-0.5.8/dimples/edge/shared.py` & `dimples-1.0.0/dimples/edge/shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     # load config from file
     config = Config.load(file=ini_file)
     print('>>> config loaded: %s => %s' % (ini_file, config))
     # OK
     return config
 
 
-def create_database(config: Config) -> Tuple[AccountDBI, MessageDBI, SessionDBI]:
+async def create_database(config: Config) -> Tuple[AccountDBI, MessageDBI, SessionDBI]:
     """ Step 2: create database """
     root = config.database_root
     public = config.database_public
     private = config.database_private
     # create database
     adb = AccountDatabase(root=root, public=public, private=private)
     mdb = MessageDatabase(root=root, public=public, private=private)
@@ -112,40 +112,40 @@
     sdb.show_info()
     # default provider
     provider = ProviderInfo.GSP
     # add neighbors
     neighbors = config.neighbors
     for node in neighbors:
         print('adding neighbor node: %s' % node)
-        sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
+        await sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
     return adb, mdb, sdb
 
 
-def create_facebook(database: AccountDBI, current_user: ID) -> ClientFacebook:
+async def create_facebook(database: AccountDBI, current_user: ID) -> ClientFacebook:
     """ Step 3: create facebook """
     facebook = ClientFacebook()
     # create archivist for facebook
     archivist = ClientArchivist(database=database)
     archivist.facebook = facebook
     facebook.archivist = archivist
     # make sure private keys exists
-    sign_key = facebook.private_key_for_visa_signature(identifier=current_user)
-    msg_keys = facebook.private_keys_for_decryption(identifier=current_user)
+    sign_key = await facebook.private_key_for_visa_signature(identifier=current_user)
+    msg_keys = await facebook.private_keys_for_decryption(identifier=current_user)
     assert sign_key is not None, 'failed to get sign key for current user: %s' % current_user
     assert len(msg_keys) > 0, 'failed to get msg keys: %s' % current_user
     print('set current user: %s' % current_user)
-    user = facebook.user(identifier=current_user)
+    user = await facebook.get_user(identifier=current_user)
     assert user is not None, 'failed to get current user: %s' % current_user
-    visa = user.visa
+    visa = await user.visa
     if visa is not None:
         # refresh visa
         now = time.time()
         visa.set_property(key='time', value=now)
         visa.sign(private_key=sign_key)
-        facebook.save_document(document=visa)
+        await facebook.save_document(document=visa)
     facebook.current_user = user
     return facebook
 
 
 def create_session(facebook: ClientFacebook, database: SessionDBI, host: str, port: int) -> ClientSession:
     # 1. create station with remote host & port
     station = Station(host=host, port=port)
```

### Comparing `dimples-0.5.8/dimples/edge/start.py` & `dimples-1.0.0/dimples/edge/start.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-
 import os
 import sys
 
 path = os.path.abspath(__file__)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 sys.path.insert(0, path)
 
-from dimples.utils import Log
+from dimples.utils import Log, Runner
 
 from dimples.edge.shared import create_config, create_database, create_facebook
 from dimples.edge.shared import GlobalVariable
 from dimples.edge.octopus import Octopus
 
 
 #
@@ -50,33 +49,35 @@
 #
 Log.LEVEL = Log.DEVELOP
 
 
 DEFAULT_CONFIG = '/etc/dim/edge.ini'
 
 
-def main():
+async def main():
     # create global variable
     shared = GlobalVariable()
     # Step 1: load config
     config = create_config(app_name='DIM Network Edge', default_config=DEFAULT_CONFIG)
     shared.config = config
     # Step 2: create database
-    adb, mdb, sdb = create_database(config=config)
+    adb, mdb, sdb = await create_database(config=config)
     shared.adb = adb
     shared.mdb = mdb
     shared.sdb = sdb
     # Step 3: create facebook
     sid = config.station_id
     assert sid is not None, 'current station ID not set: %s' % config
-    facebook = create_facebook(database=adb, current_user=sid)
+    facebook = await create_facebook(database=adb, current_user=sid)
     shared.facebook = facebook
     # create & start octopus
     host = config.station_host
     port = config.station_port
     assert host is not None and port > 0, 'station config error: %s' % config
     octopus = Octopus(shared=shared, local_host=host, local_port=port)
-    octopus.start()
+    await octopus.start()
+    while octopus.running:
+        await Runner.sleep(seconds=1.0)
 
 
 if __name__ == '__main__':
-    main()
+    Runner.sync_run(main=main())
```

### Comparing `dimples-0.5.8/dimples/group/__init__.py` & `dimples-1.0.0/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/group/admin.py` & `dimples-1.0.0/dimples/group/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def facebook(self) -> CommonFacebook:
         return self.delegate.facebook
 
     @property  # protected
     def messenger(self) -> CommonMessenger:
         return self.delegate.messenger
 
-    def update_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def update_administrators(self, administrators: List[ID], group: ID) -> bool:
         """
         Update 'administrators' in bulletin document
         (broadcast new document to all members and neighbor station)
 
         :param administrators: admin list
         :param group:          group ID
         :return: False on error
@@ -74,48 +74,48 @@
         #   0. get current user
         #
         user = facebook.current_user
         if user is None:
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
-        sign_key = facebook.private_key_for_visa_signature(identifier=me)
+        sign_key = await facebook.private_key_for_visa_signature(identifier=me)
         assert sign_key is not None, 'failed to get sign key for current user: %s' % me
         #
         #   1. check permission
         #
-        is_owner = delegate.is_owner(user=me, group=group)
+        is_owner = await delegate.is_owner(user=me, group=group)
         if not is_owner:
             self.warning(msg='cannot update administrators for group: %s, %s' % (group, me))
             return False
         #
         #   2. update document
         #
-        doc = delegate.bulletin(group)
+        doc = await delegate.get_bulletin(group)
         if doc is None:
             # TODO: create new one?
             self.error(msg='failed to get group document: %s, owner: %s' % (group, me))
             return False
         doc.set_property(key='administrators', value=ID.revert(array=administrators))
         signature = None if sign_key is None else doc.sign(private_key=sign_key)
         if signature is None:
             self.error(msg='failed to sign document for group: %s, owner: %s' % (group, me))
             return False
-        elif not delegate.save_document(document=doc):
+        elif not await delegate.save_document(document=doc):
             self.error(msg='failed to save document for group: %s' % group)
             return False
         else:
             self.info(msg='group document updated: %s' % group)
         #
         #   3. broadcast bulletin document
         #
         assert isinstance(doc, Bulletin), 'group document error: %s' % doc
-        return self.broadcast_document(document=doc)
+        return await self.broadcast_document(document=doc)
 
-    def broadcast_document(self, document: Bulletin) -> bool:
+    async def broadcast_document(self, document: Bulletin) -> bool:
         facebook = self.facebook
         messenger = self.messenger
         assert facebook is not None and messenger is not None,\
             'facebook messenger not ready: %s, %s' % (facebook, messenger)
         delegate = self.delegate
         #
         #   0. get current user
@@ -125,35 +125,35 @@
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
         #
         #   1. create 'document' command, and send to current station
         #
         group = document.identifier
-        meta = facebook.meta(identifier=group)
+        meta = await facebook.get_meta(identifier=group)
         content = DocumentCommand.response(identifier=group, meta=meta, document=document)
-        messenger.send_content(sender=me, receiver=Station.ANY, content=content, priority=1)
+        await messenger.send_content(sender=me, receiver=Station.ANY, content=content, priority=1)
         #
         #   2. check group bots
         #
-        bots = delegate.assistants(identifier=group)
+        bots = await delegate.get_assistants(identifier=group)
         if len(bots) > 0:
             # group bots exist, let them to deliver to all other members
             for item in bots:
                 if me == item:
                     self.info(msg='skip cycled message: %s' % item)
                     continue
-                messenger.send_content(sender=me, receiver=item, content=content, priority=1)
+                await messenger.send_content(sender=me, receiver=item, content=content, priority=1)
             return True
         #
         #   3. broadcast to all members
         #
-        members = delegate.members(identifier=group)
+        members = await delegate.get_members(identifier=group)
         if len(members) == 0:
             self.error(msg='failed to get group members: %s' % group)
             return False
         for item in members:
             if me == item:
                 self.info(msg='skip cycled message: %s' % item)
                 continue
-            messenger.send_content(sender=me, receiver=item, content=content, priority=1)
+            await messenger.send_content(sender=me, receiver=item, content=content, priority=1)
         return True
```

### Comparing `dimples-0.5.8/dimples/group/builder.py` & `dimples-1.0.0/dimples/group/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,43 +67,43 @@
     def facebook(self) -> CommonFacebook:
         return self.delegate.facebook
 
     @property  # protected
     def messenger(self) -> CommonMessenger:
         return self.delegate.messenger
 
-    def build_group_histories(self, group: ID) -> List[ReliableMessage]:
+    async def build_group_histories(self, group: ID) -> List[ReliableMessage]:
         """ build command list for group history:
                 0. document command
                 1. reset group command
                 2. other group commands
         """
         messages = []
         #
         #  0. build 'document' command
         #
-        doc, msg = self.build_document_command(group=group)
+        doc, msg = await self.build_document_command(group=group)
         if doc is None or msg is None:
             self.warning(msg='failed to build "document" command for group: %s' % group)
             return messages
         else:
             messages.append(msg)
         #
         #  1. append 'reset' command
         #
-        reset, msg = self.helper.reset_command_message(group=group)
+        reset, msg = await self.helper.get_reset_command_message(group=group)
         if reset is None or msg is None:
             self.warning(msg='failed to get "reset" command for group: %s' % group)
             return messages
         else:
             messages.append(msg)
         #
         #  2. append other group commands
         #
-        history = self.helper.group_histories(group=group)
+        history = await self.helper.get_group_histories(group=group)
         for pair in history:
             cmd = pair[0]
             msg = pair[1]
             if isinstance(cmd, ResetCommand):
                 # 'reset' command already add to the front
                 # assert len(messages) == 2, 'group history error: %d, %s' % (len(history), group)
                 self.info(msg='skip "reset" command for group: %s' % group)
@@ -118,50 +118,50 @@
                 if is_before(old_time=reset.time, new_time=cmd.time):
                     self.warning('expired "%s" command in group: %s, sender: %s' % (cmd.cmd, group, msg.sender))
                     continue
             messages.append(msg)
         # OK
         return messages
 
-    def build_document_command(self, group: ID) -> Tuple[Optional[Document], Optional[ReliableMessage]]:
+    async def build_document_command(self, group: ID) -> Tuple[Optional[Document], Optional[ReliableMessage]]:
         """ create broadcast 'document' command """
         user = self.facebook.current_user
-        doc = self.delegate.bulletin(group)
+        doc = await self.delegate.get_bulletin(group)
         if user is None or doc is None:
             assert user is not None, 'failed to get current user'
             self.error(msg='document not found for group: %s' % group)
             return None, None
         me = user.identifier
-        meta = self.delegate.meta(identifier=group)
+        meta = await self.delegate.get_meta(identifier=group)
         cmd = DocumentCommand.response(identifier=group, meta=meta, document=doc)
-        msg = self.__pack_broadcast_message(sender=me, content=cmd)
+        msg = await self.__pack_broadcast_message(sender=me, content=cmd)
         return doc, msg
 
-    def builder_reset_command(self, group: ID,
-                              members: Optional[List[ID]]) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+    async def builder_reset_command(self, group: ID, members: Optional[List[ID]]) \
+            -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
         """ create broadcast 'reset' group command with newest member list """
         user = self.facebook.current_user
-        owner = self.delegate.owner(identifier=group)
+        owner = await self.delegate.get_owner(identifier=group)
         if user is None or owner is None:
             assert user is not None, 'failed to get current user'
             self.error(msg='owner not found for group: %s' % group)
             return None, None
         me = user.identifier
         if owner != me:
-            admins = self.delegate.administrators(group=group)
+            admins = await self.delegate.get_administrators(group=group)
             if me not in admins:
                 self.warning(msg='not permit to build "reset" command for group: %s, %s' % (group, me))
                 return None, None
         if members is None:
-            self.delegate.members(identifier=group)
+            await self.delegate.get_members(identifier=group)
         cmd = GroupCommand.reset(group=group, members=members)
-        msg = self.__pack_broadcast_message(sender=me, content=cmd)
+        msg = await self.__pack_broadcast_message(sender=me, content=cmd)
         return cmd, msg
 
-    def __pack_broadcast_message(self, sender: ID, content: Content):
+    async def __pack_broadcast_message(self, sender: ID, content: Content):
         envelope = Envelope.create(sender=sender, receiver=ANYONE)
         i_msg = InstantMessage.create(head=envelope, body=content)
-        s_msg = self.messenger.encrypt_message(msg=i_msg)
+        s_msg = await self.messenger.encrypt_message(msg=i_msg)
         assert s_msg is not None, 'failed to encrypt message: %s' % envelope
-        r_msg = self.messenger.sign_message(msg=s_msg)
+        r_msg = await self.messenger.sign_message(msg=s_msg)
         assert r_msg is not None, 'failed to sign message: %s' % envelope
         return r_msg
```

### Comparing `dimples-0.5.8/dimples/group/delegate.py` & `dimples-1.0.0/dimples/group/delegate.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 
     @property  # Override
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
         assert isinstance(transceiver, CommonMessenger), 'messenger error: %s' % transceiver
         return transceiver
 
-    def build_group_name(self, members: List[ID]) -> str:
+    async def build_group_name(self, members: List[ID]) -> str:
         count = len(members)
         if count > 0:
             facebook = self.facebook
-            text = facebook.get_name(identifier=members[0])
+            text = await facebook.get_name(identifier=members[0])
             for i in range(1, count):
-                nickname = facebook.get_name(identifier=members[i])
+                nickname = await facebook.get_name(identifier=members[i])
                 if len(nickname) == 0:
                     continue
                 text += ', %s' % nickname
                 if len(text) > 32:
                     text = text[:28]
                     return '%s ...' % text
             # OK
@@ -78,105 +78,105 @@
         assert False, 'members should not be empty here'
 
     #
     #   Entity DataSource
     #
 
     # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
-        return self.facebook.meta(identifier=identifier)
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
+        return await self.facebook.get_meta(identifier=identifier)
 
     # Override
-    def documents(self, identifier: ID) -> List[Document]:
-        return self.facebook.documents(identifier=identifier)
+    async def get_documents(self, identifier: ID) -> List[Document]:
+        return await self.facebook.get_documents(identifier=identifier)
 
-    def bulletin(self, identifier: ID) -> Optional[Bulletin]:
+    async def get_bulletin(self, identifier: ID) -> Optional[Bulletin]:
         assert identifier.is_group, 'group ID error: %s' % identifier
-        return self.facebook.bulletin(identifier=identifier)
+        return await self.facebook.get_bulletin(identifier=identifier)
 
-    def save_document(self, document: Document) -> bool:
-        return self.facebook.save_document(document=document)
+    async def save_document(self, document: Document) -> bool:
+        return await self.facebook.save_document(document=document)
 
     #
     #   Group DataSource
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
+    async def get_founder(self, identifier: ID) -> Optional[ID]:
         assert identifier.is_group, 'group ID error: %s' % identifier
-        return self.facebook.founder(identifier=identifier)
+        return await self.facebook.get_founder(identifier=identifier)
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
+    async def get_owner(self, identifier: ID) -> Optional[ID]:
         assert identifier.is_group, 'group ID error: %s' % identifier
-        return self.facebook.owner(identifier=identifier)
+        return await self.facebook.get_owner(identifier=identifier)
 
     # Override
-    def assistants(self, identifier: ID) -> List[ID]:
+    async def get_assistants(self, identifier: ID) -> List[ID]:
         assert identifier.is_group, 'group ID error: %s' % identifier
-        return self.facebook.assistants(identifier=identifier)
+        return await self.facebook.get_assistants(identifier=identifier)
 
     # Override
-    def members(self, identifier: ID) -> List[ID]:
+    async def get_members(self, identifier: ID) -> List[ID]:
         assert identifier.is_group, 'group ID error: %s' % identifier
-        return self.facebook.members(identifier=identifier)
+        return await self.facebook.get_members(identifier=identifier)
 
-    def save_members(self, members: List[ID], group: ID) -> bool:
+    async def save_members(self, members: List[ID], group: ID) -> bool:
         assert group.is_group, 'group ID error: %s' % group
         facebook = get_facebook(helper=self)
-        return facebook.save_members(members=members, group=group)
+        return await facebook.save_members(members=members, group=group)
 
     #
     #   Administrators
     #
 
-    def administrators(self, group: ID) -> List[ID]:
+    async def get_administrators(self, group: ID) -> List[ID]:
         assert group.is_group, 'group ID error: %s' % group
         facebook = get_facebook(helper=self)
-        return facebook.administrators(group=group)
+        return await facebook.get_administrators(group=group)
 
-    def save_administrators(self, administrators: List[ID], group: ID) -> bool:
+    async def save_administrators(self, administrators: List[ID], group: ID) -> bool:
         assert group.is_group, 'group ID error: %s' % group
         facebook = get_facebook(helper=self)
-        return facebook.save_administrators(administrators, group=group)
+        return await facebook.save_administrators(administrators, group=group)
 
     #
     #   Membership
     #
 
-    def is_founder(self, user: ID, group: ID) -> bool:
+    async def is_founder(self, user: ID, group: ID) -> bool:
         assert user.is_user and group.is_group, 'ID error: %s, %s' % (user, group)
-        founder = self.founder(identifier=group)
+        founder = await self.get_founder(identifier=group)
         if founder is not None:
             return founder == user
         # check member's public key with group's meta.key
-        g_meta = self.meta(identifier=group)
-        m_meta = self.meta(identifier=user)
+        g_meta = await self.get_meta(identifier=group)
+        m_meta = await self.get_meta(identifier=user)
         if g_meta is None or m_meta is None:
             self.warning(msg='failed to get meta for group: %s, user: %s' % (group, user))
             return False
         return g_meta.match_public_key(key=m_meta.public_key)
 
-    def is_owner(self, user: ID, group: ID) -> bool:
+    async def is_owner(self, user: ID, group: ID) -> bool:
         assert user.is_user and group.is_group, 'ID error: %s, %s' % (user, group)
-        owner = self.owner(identifier=group)
+        owner = await self.get_owner(identifier=group)
         if owner is not None:
             return owner == user
         if group.type == EntityType.GROUP:
             # this is a polylogue
-            return self.is_founder(user=user, group=group)
+            return await self.is_founder(user=user, group=group)
         raise Exception('only polylogue so far')
 
-    def is_member(self, user: ID, group: ID) -> bool:
+    async def is_member(self, user: ID, group: ID) -> bool:
         assert user.is_user and group.is_group, 'ID error: %s, %s' % (user, group)
-        members = self.members(identifier=group)
+        members = await self.get_members(identifier=group)
         return user in members
 
-    def is_administrator(self, user: ID, group: ID) -> bool:
+    async def is_administrator(self, user: ID, group: ID) -> bool:
         assert user.is_user and group.is_group, 'ID error: %s, %s' % (user, group)
-        admins = self.administrators(group=group)
+        admins = await self.get_administrators(group=group)
         return user in admins
 
-    def is_assistant(self, user: ID, group: ID) -> bool:
+    async def is_assistant(self, user: ID, group: ID) -> bool:
         assert user.is_user and group.is_group, 'ID error: %s, %s' % (user, group)
-        bots = self.assistants(identifier=group)
+        bots = await self.get_assistants(identifier=group)
         return user in bots
```

### Comparing `dimples-0.5.8/dimples/group/emitter.py` & `dimples-1.0.0/dimples/group/emitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,88 +90,88 @@
         return self.delegate.facebook
 
     @property  # protected
     def messenger(self) -> CommonMessenger:
         return self.delegate.messenger
 
     # private
-    def _attach_group_times(self, group: ID, msg: InstantMessage) -> bool:
+    async def _attach_group_times(self, group: ID, msg: InstantMessage) -> bool:
         if isinstance(msg.content, GroupCommand):
             # no need to attach times for group command
             return True
         facebook = self.facebook
-        doc = facebook.bulletin(identifier=group)
+        doc = await facebook.get_bulletin(identifier=group)
         if doc is None:
             self.error(msg='failed to get bulletin document for group: %s' % group)
             return False
         # attach group document time
         last_doc_time = doc.time
         if last_doc_time is None:
             self.error(msg='document error: %s' % doc)
             return False
         else:
             msg.set_datetime(key='GDT', value=last_doc_time)
         # attach group history time
         archivist = facebook.archivist
-        last_his_time = archivist.get_last_group_history_time(group=group)
+        last_his_time = await archivist.get_last_group_history_time(group=group)
         if last_his_time is None:
             self.error(msg='failed to get history time: %s' % group)
             return False
         else:
             msg.set_datetime(key='GHT', value=last_his_time)
         return True
 
-    def send_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
+    async def send_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
         content = msg.content
         group = content.group
         if group is None:
             self.error(msg='not a group message')
             return None
         assert msg.receiver == group, 'group message error: %s' % msg
         # attach group document & history times
         # for the receiver to check whether group info synchronized
-        ok = self._attach_group_times(group=group, msg=msg)
+        ok = await self._attach_group_times(group=group, msg=msg)
         if not ok:
             self.warning(msg='failed to attach group times: %s => %s' % (group, content))
         # TODO: if it's a file message
         #       please upload the file data first
         #       before calling this
         assert not isinstance(content, FileContent) or 'data' not in content, 'content error: %s' % content
         #
         #   1. check group bots
         #
-        bots = self.delegate.assistants(identifier=group)
+        bots = await self.delegate.get_assistants(identifier=group)
         if len(bots) > 0:
             # group bots found, forward this message to any bot to let it split for me;
             # this can reduce my jobs.
             prime = bots[0]
-            return self.__forward_message(msg=msg, bot=prime, group=group, priority=priority)
+            return await self.__forward_message(msg=msg, bot=prime, group=group, priority=priority)
         #
         #   2. check group members
         #
-        members = self.delegate.members(identifier=group)
+        members = await self.delegate.get_members(identifier=group)
         count = len(members)
         if count == 0:
             self.error(msg='failed to get members for group: %s' % group)
             return None
         # no 'assistants' found in group's bulletin document?
         # split group messages and send to all members one by one
         if count < self.SECRET_GROUP_LIMIT:
             # it is a tiny group, split this message before encrypting and signing,
             # then send this group message to all members one by one
-            success = self.__split_send_message(msg=msg, members=members, group=group, priority=priority)
+            success = await self.__split_send_message(msg=msg, members=members, group=group, priority=priority)
             self.info(msg='split %d message(s) for group: %s' % (success, group))
         else:
             self.info(msg='splitting message for %d members of group: %s' % (len(members), group))
             # encrypt and sign this message first,
             # then split and send to all members one by one
-            return self.__disperse_message(msg=msg, members=members, group=group, priority=priority)
+            return await self.__disperse_message(msg=msg, members=members, group=group, priority=priority)
 
-    def __forward_message(self, msg: InstantMessage, bot: ID, group: ID,
-                          priority: int = 0) -> Optional[ReliableMessage]:
+    async def __forward_message(self, msg: InstantMessage, bot: ID, group: ID,
+                                priority: int = 0) -> Optional[ReliableMessage]:
         """ Encrypt & sign message, then forward to the bot """
         assert bot.is_user and group.is_group, 'ID error: %s, %s' % (bot, group)
         # NOTICE: because group assistant (bot) cannot be a member of the group, so
         #         if you want to send a group command to any assistant, you must
         #         set the bot ID as 'receiver' and set the group ID in content;
         #         this means you must send it to the bot directly.
         messenger = self.messenger
@@ -182,30 +182,30 @@
         # this key will be encrypted by each member's public key, so
         # all members will received a message split by the group bot,
         # but the group bots cannot decrypt it.
         msg.set_string(key='group', value=group)
         #
         #   1. pack message
         #
-        r_msg = self.packer.encrypt_sign_message(msg=msg)
+        r_msg = await self.packer.encrypt_sign_message(msg=msg)
         if r_msg is None:
             self.error(msg='failed to encrypt & sign message: %s => %s' % (msg.sender, group))
             return None
         #
         #   2. forward the group message to any bot
         #
         content = ForwardContent.create(message=r_msg)
-        _, out = messenger.send_content(sender=None, receiver=bot, content=content, priority=priority)
+        _, out = await messenger.send_content(sender=None, receiver=bot, content=content, priority=priority)
         if out is None:
             self.error(msg='failed to forward message for group: %s, bot: %s' % (group, bot))
         # OK, return the forwarding message
         return r_msg
 
-    def __disperse_message(self, msg: InstantMessage, members: List[ID], group: ID,
-                           priority: int = 0) -> Optional[ReliableMessage]:
+    async def __disperse_message(self, msg: InstantMessage, members: List[ID], group: ID,
+                                 priority: int = 0) -> Optional[ReliableMessage]:
         """ Encrypt & sign message, then disperse to all members """
         assert group.is_group, 'group ID error: %s' % group
         # assert 'group' not in msg, 'should not happen'
         messenger = self.messenger
         # NOTICE: there are too many members in this group
         #         if we still hide the group ID, the cost will be very high.
         #     so,
@@ -215,35 +215,35 @@
         #         with the accurate direction: (sender -> group)
         msg.set_string(key='group', value=group)
 
         sender = msg.sender
         #
         #   1. pack message
         #
-        r_msg = self.packer.encrypt_sign_message(msg=msg)
+        r_msg = await self.packer.encrypt_sign_message(msg=msg)
         if r_msg is None:
             self.error(msg='failed to encrypt & sign message: %s => %s' % (sender, group))
             return None
         #
         #   2. split messages
         #
         messages = self.packer.split_reliable_message(msg=r_msg, members=members)
         for item in messages:
             receiver = item.receiver
             if sender == receiver:
                 self.error(msg='cycled message: %s => %s, %s' % (sender, receiver, group))
                 continue
-            ok = messenger.send_reliable_message(msg=item, priority=priority)
+            ok = await messenger.send_reliable_message(msg=item, priority=priority)
             if not ok:
                 # assert ok, 'failed to send message: %s => %s, %s' % (sender, receiver, group)
                 self.error(msg='failed to send message: %s => %s, %s' % (sender, receiver, group))
         # sent
         return r_msg
 
-    def __split_send_message(self, msg: InstantMessage, members: List[ID], group: ID, priority: int = 0) -> int:
+    async def __split_send_message(self, msg: InstantMessage, members: List[ID], group: ID, priority: int = 0) -> int:
         """ Split and send (encrypt + sign) group messages to all members one by one """
         assert group.is_group, 'group ID error: %s' % group
         assert 'group' not in msg, 'should not happen'
         messenger = self.messenger
         #
         # NOTICE: this is a tiny group
         #         I suggest NOT to expose the group ID to maximize its privacy,
@@ -262,14 +262,14 @@
             receiver = item.receiver
             if sender == receiver:
                 self.error(msg='cycled message: %s => %s, %s' % (sender, receiver, group))
                 continue
             #
             #   2. send message
             #
-            r_msg = messenger.send_instant_message(msg=item, priority=priority)
+            r_msg = await messenger.send_instant_message(msg=item, priority=priority)
             if r_msg is None:
                 self.error(msg='failed to send message: %s => %s, %s' % (sender, receiver, group))
                 continue
             success += 1
         # done!
         return success
```

### Comparing `dimples-0.5.8/dimples/group/helper.py` & `dimples-1.0.0/dimples/group/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def database(self) -> AccountDBI:
         return self.delegate.facebook.archivist.database
 
     #
     #   Group History Command
     #
 
-    def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
+    async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
         if self.is_expired(content=content):
             self.warning(msg='drop expired command: %s, %s => %s' % (content.cmd, message.sender, group))
             return False
         # check command time
         cmd_time = content.time
         if cmd_time is None:
             self.error(msg='group command error: %s' % content)
@@ -75,48 +75,48 @@
             if cmd_time > current:
                 self.error(msg='group command time error: %s, %s' % (cmd_time, content))
                 return False
         # update group history
         db = self.database
         if isinstance(content, ResetCommand):
             self.warning(msg='cleaning group history for "reset" command: %s => %s' % (message.sender, group))
-            db.clear_group_member_histories(group=group)
-        return db.save_group_history(group=group, content=content, message=message)
+            await db.clear_group_member_histories(group=group)
+        return await db.save_group_history(group=group, content=content, message=message)
 
-    def group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
+    async def get_group_histories(self, group: ID) -> List[Tuple[GroupCommand, ReliableMessage]]:
         db = self.database
-        return db.group_histories(group=group)
+        return await db.get_group_histories(group=group)
 
-    def reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
+    async def get_reset_command_message(self, group: ID) -> Tuple[Optional[ResetCommand], Optional[ReliableMessage]]:
         db = self.database
-        return db.reset_command_message(group=group)
+        return await db.get_reset_command_message(group=group)
 
-    def clear_group_member_histories(self, group: ID) -> bool:
+    async def clear_group_member_histories(self, group: ID) -> bool:
         db = self.database
-        return db.clear_group_member_histories(group=group)
+        return await db.clear_group_member_histories(group=group)
 
-    def clear_group_admin_histories(self, group: ID) -> bool:
+    async def clear_group_admin_histories(self, group: ID) -> bool:
         db = self.database
-        return db.clear_group_admin_histories(group=group)
+        return await db.clear_group_admin_histories(group=group)
 
-    def is_expired(self, content: GroupCommand) -> bool:
+    async def is_expired(self, content: GroupCommand) -> bool:
         """ check command time
             (all group commands received must after the cached 'reset' command)
         """
         group = content.group
         assert group is not None, 'group content error: %s' % content
         if isinstance(content, ResignCommand):
             # administrator command, check with document time
-            doc = self.delegate.bulletin(group)
+            doc = await self.delegate.get_bulletin(group)
             if doc is None:
                 self.error(msg='group document not exists: %s' % group)
                 return True
             return is_before(old_time=doc.time, new_time=content.time)
         # membership command, check with reset command
-        cmd, _ = self.reset_command_message(group=group)
+        cmd, _ = await self.get_reset_command_message(group=group)
         if cmd is None:  # or msg is None:
             return False
         return is_before(old_time=cmd.time, new_time=content.time)
 
     # noinspection PyMethodMayBeStatic
     def members_from_command(self, content: GroupCommand) -> List[ID]:
         # get from 'members'
```

### Comparing `dimples-0.5.8/dimples/group/manager.py` & `dimples-1.0.0/dimples/group/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def messenger(self) -> CommonMessenger:
         return self.__delegate.messenger
 
     @property  # protected
     def database(self) -> AccountDBI:
         return self.__delegate.facebook.archivist.database
 
-    def create_group(self, members: List[ID]) -> Optional[ID]:
+    async def create_group(self, members: List[ID]) -> Optional[ID]:
         """
         Create new group with members
         (broadcast document & members to all members and neighbor station)
 
         :param members: initial group members
         :return: new group ID
         """
@@ -121,39 +121,39 @@
             # put me in the first position
             members.insert(0, founder)
         elif pos > 0:
             # move me to the front
             members.pop(pos)
             members.insert(0, founder)
         # generate group name
-        title = self.delegate.build_group_name(members=members)
+        title = await self.delegate.build_group_name(members=members)
         #
         #   2. create group with name
         #
         register = Register(database=self.database)
-        group = register.create_group(founder=founder, name=title)
+        group = await register.create_group(founder=founder, name=title)
         self.info(msg='new group: %s (%s), founder: %s' % (group, title, founder))
         #
         #   3. upload meta+document to neighbor station(s)
         #   DISCUSS: should we let the neighbor stations know the group info?
         #
-        meta = self.delegate.meta(identifier=group)
-        doc = self.delegate.bulletin(group)
+        meta = await self.delegate.get_meta(identifier=group)
+        doc = await self.delegate.get_bulletin(group)
         if doc is not None:
             content = DocumentCommand.response(identifier=group, meta=meta, document=doc)
         elif meta is not None:
             content = MetaCommand.response(identifier=group, meta=meta)
         else:
             self.error(msg='failed to get group info: %s' % group)
             return None
-        self.__send_command(content=content, receiver=Station.ANY)      # to neighbor(s)
+        await self.__send_command(content=content, receiver=Station.ANY)      # to neighbor(s)
         #
         #   4. create & broadcast 'reset' group command with new members
         #
-        if self.reset_members(members=members, group=group):
+        if await self.reset_members(members=members, group=group):
             self.info(msg='created group with %d members: %s' % (len(members), group))
         else:
             self.error(msg='failed to create group with %d members: %s' % (len(members), group))
         return group
 
     """
         DISCUSS: should we let the neighbor stations know the group info?
@@ -166,15 +166,15 @@
                 
             (B) but, if we don't let the station knows it,
                 then we must shared the group info with our members themselves;
                 and if none of them is online, you cannot get the newest info
                 immediately until someone online again.
     """
 
-    def reset_members(self, members: List[ID], group: ID) -> bool:
+    async def reset_members(self, members: List[ID], group: ID) -> bool:
         """
         Reset group members
         (broadcast new group history to all members)
 
         :param members: new member list
         :param group:   group ID
         :return: False on error
@@ -186,72 +186,72 @@
         user = self.facebook.current_user
         if user is None:
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
         # check member list
         first = members[0]
-        ok = self.delegate.is_owner(user=first, group=group)
+        ok = await self.delegate.is_owner(user=first, group=group)
         if not ok:
             self.error(msg='group owner must be the first member: %s' % group)
             return False
         # member list OK, check expelled members
-        old_members = self.delegate.members(identifier=group)
+        old_members = await self.delegate.get_members(identifier=group)
         expel_list = []
         for item in old_members:
             if item not in members:
                 expel_list.append(item)
         #
         #   1. check permission
         #
         is_owner = me == first
-        is_admin = self.delegate.is_administrator(user=me, group=group)
-        is_bot = self.delegate.is_assistant(user=me, group=group)
+        is_admin = await self.delegate.is_administrator(user=me, group=group)
+        is_bot = await self.delegate.is_assistant(user=me, group=group)
         can_reset = is_owner or is_admin
         if not can_reset:
             self.error(msg='cannot reset members of group: %s' % group)
             return False
         # only the owner or admin can reset group member
         assert not is_bot, 'group bot cannot reset members: %s, %s' % (group, me)
         #
         #   2. build 'reset' command
         #
-        reset, msg = self.builder.builder_reset_command(group=group, members=members)
+        reset, msg = await self.builder.builder_reset_command(group=group, members=members)
         if reset is None or msg is None:
             self.error(msg='failed to build "reset" command for group: %s' % group)
             return False
         #
         #   3. save 'reset' command, and update new members
         #
-        if not self.helper.save_group_history(group=group, content=reset, message=msg):
+        if not await self.helper.save_group_history(group=group, content=reset, message=msg):
             self.error(msg='failed to save "reset" command for group: %s' % group)
             return False
-        elif not self.delegate.save_members(members=members, group=group):
+        elif not await self.delegate.save_members(members=members, group=group):
             self.error(msg='failed to update members of group: %s' % group)
             return False
         else:
             self.info(msg='group members updated: %s, %d' % (group, len(members)))
         #
         #   4. forward all group history
         #
-        messages = self.builder.build_group_histories(group=group)
+        messages = await self.builder.build_group_histories(group=group)
         forward = ForwardContent.create(messages=messages)
-        bots = self.delegate.assistants(identifier=group)
+        bots = await self.delegate.get_assistants(identifier=group)
         if len(bots) > 0:
             # let the group bots know the newest member ID list,
             # so they can split group message correctly for us.
-            return self.__send_command(content=forward, members=bots)   # to all assistants
+            return await self.__send_command(content=forward, members=bots)   # to all assistants
         else:
             # group bots not exist,
             # send the command to all members
-            self.__send_command(content=forward, members=members)       # to new members
-            self.__send_command(content=forward, members=expel_list)    # to removed members
+            await self.__send_command(content=forward, members=members)       # to new members
+            await self.__send_command(content=forward, members=expel_list)    # to removed members
         return True
 
-    def invite_members(self, members: List[ID], group: ID) -> bool:
+    async def invite_members(self, members: List[ID], group: ID) -> bool:
         """
         Invite new members to this group
 
 
         :param members: inviting member list
         :param group:   group ID
         :return: False on error
@@ -262,63 +262,63 @@
         #
         user = self.facebook.current_user
         if user is None:
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
 
-        old_members = self.delegate.members(identifier=group)
-        is_owner = self.delegate.is_owner(user=me, group=group)
-        is_admin = self.delegate.is_administrator(user=me, group=group)
-        is_member = self.delegate.is_member(user=me, group=group)
+        old_members = await self.delegate.get_members(identifier=group)
+        is_owner = await self.delegate.is_owner(user=me, group=group)
+        is_admin = await self.delegate.is_administrator(user=me, group=group)
+        is_member = await self.delegate.is_member(user=me, group=group)
         #
         #   1. check permission
         #
         can_reset = is_owner or is_admin
         if can_reset:
             all_members = old_members.copy()
             for item in members:
                 if item not in all_members:
                     all_members.append(item)
-            return self.reset_members(members=all_members, group=group)
+            return await self.reset_members(members=all_members, group=group)
         elif not is_member:
             self.error(msg='cannot invite member into group: %s' % group)
             return False
         # invited by ordinary member
 
         #
         #   2. build 'invite' command
         #
         invite = GroupCommand.invite(group=group, members=members)
-        r_msg = self.packer.pack_message(content=invite, sender=me)
+        r_msg = await self.packer.pack_message(content=invite, sender=me)
         if r_msg is None:
             self.error(msg='failed to build "invite" command for group: %s' % group)
             return False
-        elif not self.helper.save_group_history(group=group, content=invite, message=r_msg):
+        elif not await self.helper.save_group_history(group=group, content=invite, message=r_msg):
             self.error(msg='failed to save "invite" command for group: %s' % group)
             return False
         forward = ForwardContent.create(message=r_msg)
         #
         #   3. forward group command(s)
         #
-        bots = self.delegate.assistants(identifier=group)
+        bots = await self.delegate.get_assistants(identifier=group)
         if len(bots) > 0:
             # let the group bots know the newest member ID list,
             # so they can split group message correctly for us.
-            return self.__send_command(content=forward, members=bots)   # to all assistants
+            return await self.__send_command(content=forward, members=bots)   # to all assistants
         # forward 'invite' to old members
-        self.__send_command(content=forward, members=old_members)       # to old members
+        await self.__send_command(content=forward, members=old_members)       # to old members
         # forward all group history to new members
-        messages = self.builder.build_group_histories(group=group)
+        messages = await self.builder.build_group_histories(group=group)
         forward = ForwardContent.create(messages=messages)
         # TODO: remove that members already exist before sending?
-        self.__send_command(content=forward, members=members)           # to new members
+        await self.__send_command(content=forward, members=members)           # to new members
         return True
 
-    def quit_group(self, group: ID) -> bool:
+    async def quit_group(self, group: ID) -> bool:
         """
         Quit from this group
         (broadcast a 'quit' command to all members)
 
         :param group: group ID
         :return: False on error
         """
@@ -328,19 +328,19 @@
         #
         user = self.facebook.current_user
         if user is None:
             self.error(msg='failed to get current user')
             return False
         me = user.identifier
 
-        members = self.delegate.members(identifier=group)
+        members = await self.delegate.get_members(identifier=group)
         assert len(members) > 0, 'failed to get members for group: %s' % group
-        is_owner = self.delegate.is_owner(user=me, group=group)
-        is_admin = self.delegate.is_administrator(user=me, group=group)
-        is_bot = self.delegate.is_assistant(user=me, group=group)
+        is_owner = await self.delegate.is_owner(user=me, group=group)
+        is_admin = await self.delegate.is_administrator(user=me, group=group)
+        is_bot = await self.delegate.is_assistant(user=me, group=group)
         is_member = me in members
         #
         #   1. check permission
         #
         if is_owner:
             self.warning(msg='owner cannot quit from group: %s' % group)
             return False
@@ -351,41 +351,41 @@
         #
         #   2. update local storage
         #
         if is_member:
             self.warning(msg='quitting group: %s, %s' % (group, me))
             new_members = members.copy()
             new_members.remove(me)
-            ok = self.delegate.save_members(members=new_members, group=group)
+            ok = await self.delegate.save_members(members=new_members, group=group)
             assert ok, 'failed to save members for group: %s' % group
             members = new_members
         else:
             self.warning(msg='members not in group: %s, %s' % (group, me))
         #
         #   3. build 'quit' command
         #
         content = GroupCommand.quit(group=group)
-        r_msg = self.packer.pack_message(content=content, sender=me)
+        r_msg = await self.packer.pack_message(content=content, sender=me)
         if r_msg is None:
             self.error(msg='failed to pack group message: %s' % group)
             return False
         forward = ForwardContent.create(message=r_msg)
         #
         #   4. forward 'quit' command
         #
-        bots = self.delegate.assistants(identifier=group)
+        bots = await self.delegate.get_assistants(identifier=group)
         if len(bots) > 0:
             # let the group bots know the newest member ID list,
             # so they can split group message correctly for us.
-            return self.__send_command(content=forward, members=bots)   # to group bots
+            return await self.__send_command(content=forward, members=bots)   # to group bots
         # group bots not exist,
         # send the command to all members directly
-        return self.__send_command(content=forward, members=members)    # to all members
+        return await self.__send_command(content=forward, members=members)    # to all members
 
-    def __send_command(self, content: Content, receiver: ID = None, members: List[ID] = None) -> bool:
+    async def __send_command(self, content: Content, receiver: ID = None, members: List[ID] = None) -> bool:
         if receiver is not None:
             assert members is None, 'params error: %s, %s' % (receiver, members)
             members = [receiver]
         elif members is None:
             # assert False, 'params error'
             return False
         # 1. get sender
@@ -396,15 +396,15 @@
         me = user.identifier
         # 2. send to all receivers
         messenger = self.messenger
         for receiver in members:
             if me == receiver:
                 self.info(msg='skip cycled message: %s => %s' % (me, receiver))
                 continue
-            messenger.send_content(sender=me, receiver=receiver, content=content, priority=1)
+            await messenger.send_content(sender=me, receiver=receiver, content=content, priority=1)
         return True
 
 
 def find(item, array: List) -> int:
     pos = 0
     for e in array:
         if e == item:
```

### Comparing `dimples-0.5.8/dimples/group/packer.py` & `dimples-1.0.0/dimples/group/packer.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,30 @@
     def delegate(self) -> GroupDelegate:
         return self.__delegate
 
     @property  # protected
     def messenger(self) -> Messenger:
         return self.delegate.messenger
 
-    def pack_message(self, content: Content, sender: ID) -> Optional[ReliableMessage]:
+    async def pack_message(self, content: Content, sender: ID) -> Optional[ReliableMessage]:
         """ Pack as broadcast message """
         envelope = Envelope.create(sender=sender, receiver=ANYONE)
         msg = InstantMessage.create(head=envelope, body=content)
         msg.set_string(key='group', value=content.group)  # expose group ID
-        return self.encrypt_sign_message(msg=msg)
+        return await self.encrypt_sign_message(msg=msg)
 
-    def encrypt_sign_message(self, msg: InstantMessage) -> Optional[ReliableMessage]:
+    async def encrypt_sign_message(self, msg: InstantMessage) -> Optional[ReliableMessage]:
         messenger = self.messenger
         # encrypt for receiver
-        s_msg = messenger.encrypt_message(msg=msg)
+        s_msg = await messenger.encrypt_message(msg=msg)
         if s_msg is None:
             self.error(msg='failed to encrypt message: %s => %s, %s' % (msg.sender, msg.receiver, msg.get('group')))
             return None
         # sign for sender
-        r_msg = messenger.sign_message(msg=s_msg)
+        r_msg = await messenger.sign_message(msg=s_msg)
         if r_msg is None:
             self.error(msg='failed to sign message: %s => %s, %s' % (msg.sender, msg.receiver, msg.get('group')))
             return None
         return r_msg
 
     def split_instant_message(self, msg: InstantMessage, members: List[ID]) -> List[InstantMessage]:
         messages = []
```

### Comparing `dimples-0.5.8/dimples/register/__init__.py` & `dimples-1.0.0/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/register/base.py` & `dimples-1.0.0/dimples/register/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,51 +135,51 @@
         doc = self.__doc
         print('!!!')
         print('!!! ID: %s' % identifier)
         print('!!!')
         print('!!! meta type: %d, document type: %s, name: "%s"' % (meta.type, doc.type, doc.name))
         print('!!!')
 
-    def load_info(self, identifier: ID) -> Tuple[Optional[Meta], Optional[Document]]:
+    async def load_info(self, identifier: ID) -> Tuple[Optional[Meta], Optional[Document]]:
         assert self.__id is None, 'ID exists: %s' % self.__id
         assert self.__meta is None, 'meta exists: %s' % self.__meta
         assert self.__doc is None, 'document exists: %s' % self.__doc
         db = self.__db
-        meta = db.meta(identifier=identifier)
+        meta = await db.get_meta(identifier=identifier)
         if meta is None:
             self.error(msg='failed to load meta: %s' % identifier)
             return None, None
-        documents = db.documents(identifier=identifier)
+        documents = await db.get_documents(identifier=identifier)
         if len(documents) == 0:
             self.error(msg='failed to load documents: %s' % identifier)
             return meta, None
         doc = DocumentHelper.last_document(documents=documents)
         self.__id = identifier
         self.__meta = meta
         self.__doc = doc
         return meta, doc
 
-    def save_meta(self) -> Optional[Tuple[ID, Meta]]:
+    async def save_meta(self) -> Optional[Tuple[ID, Meta]]:
         identifier = self.__id
         meta = self.__meta
         db = self.__db
-        if db.save_meta(meta=meta, identifier=identifier):
+        if await db.save_meta(meta=meta, identifier=identifier):
             return identifier, meta
         else:
             self.error(msg='failed to save meta: %s, %s' % (identifier, meta))
 
-    def save_document(self) -> Optional[Document]:
+    async def save_document(self) -> Optional[Document]:
         doc = self.__doc
         db = self.__db
-        if db.save_document(document=doc):
+        if await db.save_document(document=doc):
             return doc
         else:
             self.error(msg='failed to save document: %s, %s' % (doc.identifier, doc))
 
-    def update(self, exists: bool = False) -> Optional[Document]:
+    async def update(self, exists: bool = False) -> Optional[Document]:
         doc = self.edit()
         assert doc is not None, 'failed to edit document'
         # TODO: sign & save
         return doc
 
     @abstractmethod
     def edit(self) -> Optional[Document]:
```

### Comparing `dimples-0.5.8/dimples/register/ext.py` & `dimples-1.0.0/dimples/register/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,19 +57,19 @@
         assert self.__founder is None, 'founder exists: %s' % self.__founder
         value = input('>>> please input group founder: ')
         value = value.strip()
         if len(value) > 0:
             self.__founder = ID.parse(identifier=value)
         return self.__founder
 
-    def load_founder(self, founder: ID) -> Optional[SignKey]:
+    async def load_founder(self, founder: ID) -> Optional[SignKey]:
         assert self.__founder is None or self.__founder == founder, 'another founder exists: %s' % self.__founder
         assert self.__id_pri_key is None, 'private key exists: %s' % self.__id_pri_key
         db = self.database
-        id_key = db.private_key_for_visa_signature(user=founder)
+        id_key = await db.private_key_for_visa_signature(user=founder)
         if id_key is None:
             self.error(msg='failed to load id key: %s' % founder)
             return None
         self.__founder = founder
         self.__id_pri_key = id_key
         return id_key
 
@@ -80,28 +80,28 @@
         assert meta is not None, 'failed to generate meta'
         identifier = self.generate_identifier(network=network)
         doc = self.generate_document(doc_type=Document.BULLETIN)
         assert doc.identifier == identifier, 'ID not match: %s' % identifier
         return doc
 
     # Override
-    def update(self, exists: bool = False) -> Optional[Document]:
+    async def update(self, exists: bool = False) -> Optional[Document]:
         doc = self.edit()
         assert isinstance(doc, Bulletin), 'failed to edit bulletin: %s' % doc
         # check founder & sign
         founder = doc.founder
         if founder is None:
             founder = self.__founder
             assert founder is not None, 'founder not found'
             doc.set_property(key='founder', value=str(founder))
         if doc.sign(private_key=self.__id_pri_key) is None:
             return None
         if not exists:
-            self.save_meta()
-        return self.save_document()
+            await self.save_meta()
+        return await self.save_document()
 
     # protected
     def edit(self) -> Optional[Document]:
         return self.edit_properties(fields=self.GROUP_FIELDS)
 
 
 class UserAccount(BaseAccount):
@@ -109,25 +109,25 @@
     def __init__(self, database: AccountDBI):
         super().__init__(database=database)
         # private keys
         self.__id_pri_key: Optional[PrivateKey] = None
         self.__msg_pri_keys: Optional[List[PrivateKey]] = None
 
     # Override
-    def load_info(self, identifier: ID) -> Tuple[Optional[Meta], Optional[Document]]:
+    async def load_info(self, identifier: ID) -> Tuple[Optional[Meta], Optional[Document]]:
         db = self.database
-        id_key = db.private_key_for_visa_signature(user=identifier)
+        id_key = await db.private_key_for_visa_signature(user=identifier)
         if id_key is None:
             self.error(msg='failed to load id key: %s' % identifier)
             return None, None
-        msg_keys = db.private_keys_for_decryption(user=identifier)
+        msg_keys = await db.private_keys_for_decryption(user=identifier)
         if len(msg_keys) == 0:
             self.error(msg='failed to load msg keys: %s' % identifier)
             return None, None
-        meta, doc = super().load_info(identifier=identifier)
+        meta, doc = await super().load_info(identifier=identifier)
         if doc is None:
             return meta, None
         self.__id_pri_key = id_key
         self.__msg_pri_keys = msg_keys
         return meta, doc
 
     # Override
@@ -137,24 +137,24 @@
         id_key = self.__id_pri_key
         msg_keys = self.__msg_pri_keys
         algor = None if id_key is None else id_key.algorithm
         array = [] if msg_keys is None else [key.algorithm for key in msg_keys]
         print('!!! private key: %s, msg keys: %s' % (algor, array))
         print('!!!')
 
-    def save_private_keys(self) -> Tuple[PrivateKey, List[PrivateKey]]:
+    async def save_private_keys(self) -> Tuple[PrivateKey, List[PrivateKey]]:
         id_pri_key = self.__id_pri_key
         msg_pri_keys = self.__msg_pri_keys
         assert id_pri_key is not None and len(msg_pri_keys) > 0, 'private keys not found'
         identifier = self.identifier
         assert identifier is not None, 'ID not found'
         db = self.database
-        db.save_private_key(key=id_pri_key, user=identifier, key_type=PrivateKeyStorage.ID_KEY_TAG)
+        await db.save_private_key(key=id_pri_key, user=identifier, key_type=PrivateKeyStorage.ID_KEY_TAG)
         for s_key in msg_pri_keys:
-            db.save_private_key(key=s_key, user=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
+            await db.save_private_key(key=s_key, user=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
         return id_pri_key, msg_pri_keys
 
     # private
     def generate_keys(self) -> Tuple[PrivateKey, List[PrivateKey]]:
         if self.__id_pri_key is None:
             self.__id_pri_key = PrivateKey.generate(algorithm=PrivateKey.ECC)
         if self.__msg_pri_keys is None:
@@ -169,25 +169,25 @@
         identifier = self.generate_identifier(network=network)
         doc = self.generate_document(doc_type=Document.VISA)
         assert isinstance(doc, Visa), 'visa error: %s' % doc
         assert doc.identifier == identifier, 'ID not match: %s' % identifier
         return doc
 
     # Override
-    def update(self, exists: bool = False) -> Optional[Document]:
+    async def update(self, exists: bool = False) -> Optional[Document]:
         doc = self.edit()
         assert isinstance(doc, Visa), 'failed to edit visa: %s' % doc
         # update visa.key and sign
         doc.public_key = self.__msg_pri_keys[0].public_key
         if doc.sign(private_key=self.__id_pri_key) is None:
             return None
         if not exists:
-            self.save_private_keys()
-            self.save_meta()
-        return self.save_document()
+            await self.save_private_keys()
+            await self.save_meta()
+        return await self.save_document()
 
     # protected
     def edit(self) -> Optional[Document]:
         return self.edit_properties(fields=self.USER_FIELDS)
 
 
 class BotAccount(UserAccount):
```

### Comparing `dimples-0.5.8/dimples/register/run.py` & `dimples-1.0.0/dimples/register/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-
 import os
 import sys
 import getopt
 
 from dimsdk import ID
 
 path = os.path.abspath(__file__)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 sys.path.insert(0, path)
 
 from dimples.utils import Log, Config
+from dimples.utils import Runner
 from dimples.database import Storage
 
 from dimples.register.shared import GlobalVariable
 from dimples.register.shared import create_database
 from dimples.register.shared import generate, modify
 
 
@@ -70,15 +70,15 @@
     print('')
     print('optional arguments:')
     print('    --config        config file path (default: "%s")' % DEFAULT_CONFIG)
     print('    --help, -h      show this help message and exit')
     print('')
 
 
-def main():
+async def main():
     try:
         opts, args = getopt.getopt(args=sys.argv[1:],
                                    shortopts='hf:',
                                    longopts=['help', 'config='])
     except getopt.GetoptError:
         show_help()
         sys.exit(1)
@@ -101,21 +101,21 @@
         sys.exit(0)
     # load config
     config = Config.load(file=ini_file)
     # initializing
     print('[DB] init with config: %s => %s' % (ini_file, config))
     shared = GlobalVariable()
     shared.config = config
-    create_database(shared=shared)
+    await create_database(shared=shared)
     # check actions
     if len(args) == 1 and args[0] == 'generate':
-        generate(database=shared.adb)
+        await generate(database=shared.adb)
     elif len(args) == 2 and args[0] == 'modify':
         identifier = ID.parse(identifier=args[1])
         assert identifier is not None, 'ID error: %s' % args[1]
-        modify(identifier=identifier, database=shared.adb)
+        await modify(identifier=identifier, database=shared.adb)
     else:
         show_help()
 
 
 if __name__ == '__main__':
-    main()
+    Runner.sync_run(main=main())
```

### Comparing `dimples-0.5.8/dimples/register/shared.py` & `dimples-1.0.0/dimples/register/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def __init__(self):
         super().__init__()
         self.config: Optional[Config] = None
         self.adb: Optional[AccountDBI] = None
 
 
-def create_database(shared: GlobalVariable) -> AccountDBI:
+async def create_database(shared: GlobalVariable) -> AccountDBI:
     config = shared.config
     root = config.database_root
     public = config.database_public
     private = config.database_private
     # create database
     adb = AccountDatabase(root=root, public=public, private=private)
     adb.show_info()
@@ -68,39 +68,39 @@
         return StationAccount(database=database)
     elif network in [EntityType.BOT, NetworkType.BOT]:
         return BotAccount(database=database)
     else:
         return UserAccount(database=database)
 
 
-def generate(database: AccountDBI):
+async def generate(database: AccountDBI):
     print('Generating DIM account...')
     #
     #   Step 0. get entity type, meta type & meta seed (ID.name)
     #
     network = BaseAccount.get_address_type()
     version = BaseAccount.get_meta_type(address_type=network)
     seed = BaseAccount.get_meta_seed(meta_type=version, address_type=network)
     #
     #   Step 1. generate account
     #
     account = create_account(network=network, database=database)
     if isinstance(account, GroupAccount):
         founder = account.get_founder()
         assert founder is not None, 'failed to get founder'
-        account.load_founder(founder=founder)
+        await account.load_founder(founder=founder)
     account.generate(network=network, version=version, seed=seed)
     #
     #   Step 2. edit & save
     #
-    account.update()
+    await account.update()
     account.show_info()
 
 
-def modify(identifier: ID, database: AccountDBI):
+async def modify(identifier: ID, database: AccountDBI):
     print('Modifying DIM account...')
     #
     #   Step 0: check meta & document
     #
     network = identifier.type
     #
     #   Step 1: create account
@@ -111,9 +111,9 @@
         assert isinstance(doc, Bulletin), 'group document error: %s' % doc
         founder = doc.founder
         assert founder is not None, 'founder not found: %s' % doc
         account.load_founder(founder=founder)
     #
     #   Step 2. edit & save
     #
-    account.update()
+    await account.update()
     account.show_info()
```

### Comparing `dimples-0.5.8/dimples/server/__init__.py` & `dimples-1.0.0/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/server/archivist.py` & `dimples-1.0.0/dimples/server/archivist.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,94 +93,94 @@
                     if item.type == EntityType.STATION:
                         neighbors.add(item)
                 self.__neighbors = neighbors
                 self.__expires = now.timestamp + 128
             return self.__neighbors
 
     @property
-    def all_stations(self) -> List[StationInfo]:
+    async def all_stations(self) -> List[StationInfo]:
         """ get stations from database """
         dispatcher = get_dispatcher()
         db = dispatcher.sdb
         # TODO: get chosen provider
-        providers = db.all_providers()
+        providers = await db.all_providers()
         assert len(providers) > 0, 'service provider not found'
         gsp = providers[0].identifier
-        return db.all_stations(provider=gsp)
+        return await db.all_stations(provider=gsp)
 
     @property
-    def all_neighbors(self) -> Set[ID]:
+    async def all_neighbors(self) -> Set[ID]:
         """ get all stations """
         neighbors = set()
         # get stations from chosen provider
-        chosen_stations = self.all_stations
+        chosen_stations = await self.all_stations
         for item in chosen_stations:
             sid = item.identifier
             if sid is None or sid.is_broadcast:
                 continue
             neighbors.add(sid)
         # get neighbor station from session server
         proactive_neighbors = self.active_stations
         for sid in proactive_neighbors:
             if sid is None or sid.is_broadcast:
                 self.error(msg='neighbor station ID error: %s' % sid)
                 continue
             neighbors.add(sid)
         return neighbors
 
-    def _broadcast_command(self, command: Command) -> bool:
+    async def _broadcast_command(self, command: Command) -> bool:
         facebook = get_facebook(archivist=self)
         messenger = get_messenger(archivist=self)
         if facebook is None or messenger is None:
             self.error(msg='twins not ready yet: %s, %s' % (facebook, messenger))
             return False
         sid = facebook.current_user.identifier
         env = Envelope.create(sender=sid, receiver=Station.EVERY)
         i_msg = InstantMessage.create(head=env, body=command)
         # pack & deliver message
-        s_msg = messenger.encrypt_message(msg=i_msg)
-        r_msg = messenger.sign_message(msg=s_msg)
+        s_msg = await messenger.encrypt_message(msg=i_msg)
+        r_msg = await messenger.sign_message(msg=s_msg)
         # dispatch
         dispatcher = get_dispatcher()
-        neighbors = self.all_neighbors
+        neighbors = await self.all_neighbors
         # avoid the new recipients redirect it to same targets
         r_msg['recipients'] = ID.revert(neighbors)
         for receiver in neighbors:
             if receiver == sid:
                 self.debug(msg='skip cycled message: %s -> %s' % (sid, receiver))
                 continue
-            dispatcher.deliver_message(msg=r_msg, receiver=receiver)
+            await dispatcher.deliver_message(msg=r_msg, receiver=receiver)
         return len(neighbors) > 0
 
     # protected
     def is_documents_respond_expired(self, identifier: ID, force: bool) -> bool:
         return self.__document_responses.is_expired(key=identifier, force=force)
 
     def set_last_active_member(self, member: ID, group: ID):
         self.__last_active_members[group] = member
 
     # Override
-    def query_meta(self, identifier: ID) -> bool:
+    async def query_meta(self, identifier: ID) -> bool:
         if not self.is_meta_query_expired(identifier=identifier):
             # query not expired yet
             self.info(msg='meta query not expired yet: %s' % identifier)
             return False
         self.info(msg='querying meta for: %s' % identifier)
         command = MetaCommand.query(identifier=identifier)
-        return self._broadcast_command(command=command)
+        return await self._broadcast_command(command=command)
 
     # Override
-    def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    async def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
         if not self.is_documents_query_expired(identifier=identifier):
             # query not expired yet
             self.info(msg='document query not expired yet: %s' % identifier)
             return False
-        last_time = self.get_last_document_time(identifier=identifier, documents=documents)
+        last_time = await self.get_last_document_time(identifier=identifier, documents=documents)
         self.info(msg='querying document for: %s, last time: %s' % (identifier, last_time))
         command = DocumentCommand.query(identifier=identifier, last_time=last_time)
-        return self._broadcast_command(command=command)
+        return await self._broadcast_command(command=command)
 
     # Override
-    def query_members(self, group: ID, members: List[ID]) -> bool:
+    async def query_members(self, group: ID, members: List[ID]) -> bool:
         # station will never process group info
         self.error(msg='DON\'t call me!')
         return False
```

### Comparing `dimples-0.5.8/dimples/server/cpu/__init__.py` & `dimples-1.0.0/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/server/cpu/ans.py` & `dimples-1.0.0/dimples/server/cpu/ans.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from ...utils import Log
 from ...common import AnsCommand
 
 
 class AnsCommandProcessor(BaseCommandProcessor):
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, AnsCommand), 'report command error: %s' % content
         names = content.names
         if len(names) == 0:
             text = 'ANS command error.'
             return self._respond_receipt(text=text, envelope=r_msg.envelope, content=content, extra={})
         records = {}
         missed = []
```

### Comparing `dimples-0.5.8/dimples/server/cpu/document.py` & `dimples-1.0.0/dimples/server/cpu/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,46 +52,46 @@
     @property
     def session(self) -> Session:
         messenger = self.messenger
         assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
         return messenger.session
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, DocumentCommand), 'document command error: %s' % content
-        responses = super().process_content(content=content, r_msg=r_msg)
+        responses = await super().process_content(content=content, r_msg=r_msg)
         if content.document is None:
             # this is a request, check DocumentCommand & LoginCommand
             if has_document(contents=responses):
                 db = self.session.database
                 current = self.facebook.current_user
                 sid = current.identifier
                 assert db is not None, 'session DB not found'
                 assert sid is not None, 'current station not found: %s' % current
                 # forward login message after document command
-                res = forward_login_msg(doc_id=content.identifier, sender=r_msg.sender, node=sid, database=db)
+                res = await forward_login_msg(doc_id=content.identifier, sender=r_msg.sender, node=sid, database=db)
                 if res is not None:
                     responses.append(res)
         return responses
 
 
 def has_document(contents: List[Content]) -> bool:
     for item in contents:
         if isinstance(item, DocumentCommand):
             return True
 
 
-def forward_login_msg(doc_id: ID, sender: ID, node: ID, database: SessionDBI) -> Optional[ForwardContent]:
-    login_msg = get_login_msg(doc_id=doc_id, sender=sender, node=node, database=database)
+async def forward_login_msg(doc_id: ID, sender: ID, node: ID, database: SessionDBI) -> Optional[ForwardContent]:
+    login_msg = await get_login_msg(doc_id=doc_id, sender=sender, node=node, database=database)
     if login_msg is not None:
         # respond login command
         return ForwardContent.create(message=login_msg)
 
 
-def get_login_msg(doc_id: ID, sender: ID, node: ID, database: SessionDBI) -> Optional[ReliableMessage]:
+async def get_login_msg(doc_id: ID, sender: ID, node: ID, database: SessionDBI) -> Optional[ReliableMessage]:
     """
     Get login message for document command
 
     :param doc_id:   document command ID
     :param sender:   sender ID
     :param node:     current node ID
     :param database: session database
@@ -100,15 +100,15 @@
     if sender == node:
         # the station is querying itself, ignore it
         return None
     elif sender.type == EntityType.BOT:
         # no need to respond LoginCommand message to a bot,
         # just ignore it
         return None
-    cmd, msg = database.login_command_message(user=doc_id)
+    cmd, msg = await database.get_login_command_message(user=doc_id)
     if cmd is not None:
         if sender.type == EntityType.STATION:
             # this is a request from another station.
             # if the user is not roaming to this station, just ignore it,
             # let the target station to respond.
             roaming = cmd.station
             assert isinstance(roaming, dict), 'login command error: %s' % cmd
```

### Comparing `dimples-0.5.8/dimples/server/cpu/handshake.py` & `dimples-1.0.0/dimples/server/cpu/handshake.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
         assert isinstance(transceiver, CommonMessenger), 'messenger error: %s' % transceiver
         return transceiver
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, HandshakeCommand), 'handshake command error: %s' % content
         title = content.title
         if title in ['DIM?', 'DIM!']:
             # S -> C
             text = 'Command not support.'
             return self._respond_receipt(text=text, envelope=r_msg.envelope, content=content, extra={
                 'template': 'Handshake command error: title="${title}".',
@@ -72,26 +72,26 @@
         sender = r_msg.sender
         if sess_id is not None:
             assert sess_id == sender, 'sender error: %s, %s' % (sender, sess_id)
         if session.key == content.session:
             # session key match
             Log.info(msg='handshake accepted: %s, session: %s' % (sender, session.key))
             # verified success
-            handshake_accepted(identifier=sender, when=content.time, session=session, messenger=messenger)
+            await handshake_accepted(identifier=sender, when=content.time, session=session, messenger=messenger)
             res = HandshakeCommand.success(session=session.key)
         else:
             # session key not match
             # ask client to sign it with the new session key
             res = HandshakeCommand.again(session=session.key)
         res['remote_address'] = session.remote_address
         return [res]
 
 
-def handshake_accepted(identifier: ID, when: Optional[DateTime], session: Session, messenger: CommonMessenger):
+async def handshake_accepted(identifier: ID, when: Optional[DateTime], session: Session, messenger: CommonMessenger):
     from ..session_center import SessionCenter
     center = SessionCenter()
     # 1. update session ID
     center.update_session(session=session, identifier=identifier)
     # 2. update session flag
     session.set_active(active=True, when=when)
     # 3. callback
-    messenger.handshake_success()
+    await messenger.handshake_success()
```

### Comparing `dimples-0.5.8/dimples/server/cpu/login.py` & `dimples-1.0.0/dimples/server/cpu/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
         assert isinstance(transceiver, CommonMessenger), 'messenger error: %s' % transceiver
         return transceiver
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, LoginCommand), 'command error: %s' % content
         sender = content.identifier
         # 1. store login command
         session = self.messenger.session
         db = session.database
-        if not db.save_login_command_message(user=sender, content=content, msg=r_msg):
+        if not await db.save_login_command_message(user=sender, content=content, msg=r_msg):
             self.error(msg='login command error/expired: %s' % content)
             return []
         # 2. check roaming station
         current = self.facebook.current_user
         station = content.station
         roaming = ID.parse(identifier=station.get('ID'))
         # assert isinstance(roaming, ID), 'login command error: %s' % content
```

### Comparing `dimples-0.5.8/dimples/server/cpu/report.py` & `dimples-1.0.0/dimples/server/cpu/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     @property
     def session(self) -> Session:
         messenger = self.messenger
         assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
         return messenger.session
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ReportCommand), 'report command error: %s' % content
         # check session sender
         session = self.session
         sender = r_msg.sender
         if session.identifier is None:
             self.error(msg='session not login, drop report command: %s => %s' % (sender, content))
             return []
```

### Comparing `dimples-0.5.8/dimples/server/dispatcher.py` & `dimples-1.0.0/dimples/server/dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 from typing import Optional, Set, List
 
 from dimsdk import EntityType, ID, EVERYONE
 from dimsdk import Station
 from dimsdk import Content, ReceiptCommand
 from dimsdk import ReliableMessage
 
-from ..utils import Singleton, Log, Logging, Runner, Daemon
+from ..utils import Singleton, Log, Logging, Runner, DaemonRunner
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
 from ..common import ReliableMessageDBI
 from ..common import LoginCommand
 
 from .session_center import SessionCenter
 from .push import PushCenter
 from .archivist import ServerArchivist
 
 
 class MessageDeliver(ABC):
     """ Delegate for deliver message """
 
     @abstractmethod
-    def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+    async def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
         """
         Deliver message to destination
 
         :param msg:      message delivering
         :param receiver: message destination
         :return: responses
         """
@@ -129,48 +129,48 @@
     def roamer(self):  # -> Roamer
         runner = self.__roamer
         if runner is None:
             db = self.mdb
             assert db is not None, 'dispatcher not initialized'
             runner = Roamer(database=db)
             self.__roamer = runner
-            runner.start()
+            Runner.async_run(coroutine=runner.start())
         return runner
 
     def add_roaming(self, user: ID, station: ID) -> bool:
         """ Add roaming user with station """
         roamer = self.roamer
         return roamer.add_roaming(user=user, station=station)
 
     #
     #   Deliver
     #
 
     # Override
-    def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+    async def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
         """ Deliver message to destination """
         worker = self.deliver_worker
         if receiver.is_group:
             # broadcast message to neighbor stations
             # e.g.: 'stations@everywhere', 'everyone@everywhere'
-            return self.__deliver_group_message(msg=msg, receiver=receiver)
+            return await self.__deliver_group_message(msg=msg, receiver=receiver)
         elif receiver.type == EntityType.STATION:
             # message to other stations
             # station won't roam to other station, so just push for it directly
-            responses = worker.redirect_message(msg=msg, neighbor=receiver)
+            responses = await worker.redirect_message(msg=msg, neighbor=receiver)
         elif receiver.type == EntityType.BOT:
             # message to a bot
             # save message before trying to push
-            self.__save_reliable_message(msg=msg, receiver=receiver)
-            responses = worker.push_message(msg=msg, receiver=receiver)
+            await self.__save_reliable_message(msg=msg, receiver=receiver)
+            responses = await worker.push_message(msg=msg, receiver=receiver)
         else:
             # message to user
             # save message before trying to push
-            self.__save_reliable_message(msg=msg, receiver=receiver)
-            responses = worker.push_message(msg=msg, receiver=receiver)
+            await self.__save_reliable_message(msg=msg, receiver=receiver)
+            responses = await worker.push_message(msg=msg, receiver=receiver)
             if responses is None:
                 # failed to push message, user not online and not roamed to other station,
                 # push notification for the receiver
                 center = PushCenter()
                 center.push_notification(msg=msg)
         # OK
         if responses is None:
@@ -183,33 +183,33 @@
             text = 'Message received.'
             res = ReceiptCommand.create(text=text, envelope=msg.envelope)
             return [res]
         else:
             # message delivered
             return responses
 
-    def __deliver_group_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+    async def __deliver_group_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
         if receiver == Station.EVERY or receiver == EVERYONE:
             # broadcast message to neighbor stations
             # e.g.: 'stations@everywhere', 'everyone@everywhere'
             archivist = self.facebook.archivist
             assert isinstance(archivist, ServerArchivist)
-            candidates = archivist.all_neighbors
+            candidates = await archivist.all_neighbors
             if len(candidates) == 0:
                 self.warning(msg='failed to get neighbors: %s' % receiver)
                 return []
             self.info(msg='forward to neighbor stations: %s -> %s' % (receiver, candidates))
-            return self.__broadcast_message(msg=msg, receiver=receiver, neighbors=candidates)
+            return await self.__broadcast_message(msg=msg, receiver=receiver, neighbors=candidates)
         else:
             self.warning(msg='unknown group: %s' % receiver)
             text = 'Group message not allow for this station'
             res = ReceiptCommand.create(text=text, envelope=msg.envelope)
             return [res]
 
-    def __broadcast_message(self, msg: ReliableMessage, receiver: ID, neighbors: Set[ID]) -> List[Content]:
+    async def __broadcast_message(self, msg: ReliableMessage, receiver: ID, neighbors: Set[ID]) -> List[Content]:
         current = self.facebook.current_user
         assert current is not None, 'failed to get current station'
         current = current.identifier
         #
         #  0. check recipients
         #
         new_recipients = set()
@@ -229,65 +229,64 @@
         all_recipients = list(old_recipients) + list(new_recipients)
         msg['recipients'] = ID.revert(all_recipients)
         #
         #  1. push to neighbor stations directly
         #
         indirect_neighbors = set()
         for target in new_recipients:
-            if session_push(msg=msg, receiver=target) == 0:
+            if await session_push(msg=msg, receiver=target) == 0:
                 indirect_neighbors.add(target)
         # remove unsuccessful items
         for item in indirect_neighbors:
             new_recipients.discard(item)
         # update 'recipients' before redirect via bridge
         self.info(msg='update recipients: %s, %s + %s' % (receiver, new_recipients, old_recipients))
         all_recipients = list(old_recipients) + list(new_recipients)
         msg['recipients'] = ID.revert(all_recipients)
         #
         #  2. push to other neighbor stations via station bridge
         #
         worker = self.deliver_worker
-        worker.redirect_message(msg=msg, neighbor=None)
+        await worker.redirect_message(msg=msg, neighbor=None)
         #
         #  OK
         #
         text = 'Message forwarded.'
         cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
         cmd['recipients'] = ID.revert(new_recipients)
         return [cmd]
 
-    def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+    async def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         if receiver.type == EntityType.STATION or msg.sender.type == EntityType.STATION:
             # no need to save station message
             return False
         elif msg.receiver.is_broadcast:
             # no need to save broadcast message
             return False
         db = self.__mdb
-        return db.cache_reliable_message(msg=msg, receiver=receiver)
+        return await db.cache_reliable_message(msg=msg, receiver=receiver)
 
 
 class RoamingInfo:
 
     def __init__(self, user: ID, station: ID):
         super().__init__()
         self.user = user
         self.station = station
 
 
-class Roamer(Runner, Logging):
+class Roamer(DaemonRunner, Logging):
     """ Delegate for redirect cached messages to roamed station """
 
     def __init__(self, database: MessageDBI):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__database = database
         # roaming (user id => station id)
         self.__queue: List[RoamingInfo] = []
         self.__lock = threading.Lock()
-        self.__daemon = Daemon(target=self)
 
     @property
     def database(self) -> Optional[MessageDBI]:
         return self.__database
 
     def __append(self, info: RoamingInfo):
         with self.__lock:
@@ -306,36 +305,33 @@
         :param station: station roamed to
         :return: False on error
         """
         info = RoamingInfo(user=user, station=station)
         self.__append(info=info)
         return True
 
-    def start(self):
-        self.__daemon.start()
-
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         info = self.__next()
         if info is None:
             # nothing to do
             return False
         receiver = info.user
         roaming = info.station
         limit = ReliableMessageDBI.CACHE_LIMIT
         try:
             db = self.database
-            cached_messages = db.reliable_messages(receiver=receiver, limit=limit)
+            cached_messages = await db.get_reliable_messages(receiver=receiver, limit=limit)
             self.debug(msg='got %d cached messages for roaming user: %s' % (len(cached_messages), receiver))
             # get deliver delegate for receiver
             dispatcher = Dispatcher()
             worker = dispatcher.deliver_worker
             # deliver cached messages one by one
             for msg in cached_messages:
-                worker.push_message(msg=msg, receiver=receiver)
+                await worker.push_message(msg=msg, receiver=receiver)
         except Exception as e:
             self.error(msg='process roaming user (%s => %s) error: %s' % (receiver, roaming, e))
         # return True to process next immediately
         return True
 
 
 class DeliverWorker(Logging):
@@ -350,40 +346,40 @@
     def database(self) -> Optional[SessionDBI]:
         return self.__database
 
     @property
     def facebook(self) -> Optional[CommonFacebook]:
         return self.__facebook
 
-    def push_message(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
+    async def push_message(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
         """
         Push message for receiver
 
         :param msg:      network message
         :param receiver: actual receiver
         :return: responses
         """
         assert receiver.is_user, 'receiver ID error: %s' % receiver
         assert receiver.type != EntityType.STATION, 'should not push message for station: %s' % receiver
         # 1. try to push message directly
-        if session_push(msg=msg, receiver=receiver) > 0:
+        if await session_push(msg=msg, receiver=receiver) > 0:
             text = 'Message delivered.'
             cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
             cmd['recipient'] = str(receiver)
             return [cmd]
         # 2. get roaming station
-        roaming = get_roaming_station(receiver=receiver, database=self.database)
+        roaming = await get_roaming_station(receiver=receiver, database=self.database)
         if roaming is None:
             # login command not found
             # return None to tell the push center to push notification for it.
             return None
         # 3. redirect message to roaming station
-        return self.redirect_message(msg=msg, neighbor=roaming)
+        return await self.redirect_message(msg=msg, neighbor=roaming)
 
-    def redirect_message(self, msg: ReliableMessage, neighbor: Optional[ID]) -> Optional[List[Content]]:
+    async def redirect_message(self, msg: ReliableMessage, neighbor: Optional[ID]) -> Optional[List[Content]]:
         """
         Redirect message to neighbor station
 
         :param msg:      network message
         :param neighbor: neighbor station
         :return: responses
         """
@@ -395,24 +391,24 @@
         assert current.type == EntityType.STATION, 'current station ID error: %s' % current
         if neighbor == current:
             self.debug(msg='same destination: %s, msg %s => %s' % (neighbor, msg.sender, msg.receiver))
             # the user is roaming to current station, but it's not online now
             # return None to tell the push center to push notification for it.
             return None
         # 1. try to push message to neighbor station directly
-        if neighbor is not None and session_push(msg=msg, receiver=neighbor) > 0:
+        if neighbor is not None and await session_push(msg=msg, receiver=neighbor) > 0:
             text = 'Message redirected.'
             cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
             cmd['neighbor'] = str(neighbor)
             return [cmd]
         # 2. push message to bridge
-        return bridge_message(msg=msg, neighbor=neighbor, bridge=current)
+        return await bridge_message(msg=msg, neighbor=neighbor, bridge=current)
 
 
-def bridge_message(msg: ReliableMessage, neighbor: Optional[ID], bridge: ID) -> List[Content]:
+async def bridge_message(msg: ReliableMessage, neighbor: Optional[ID], bridge: ID) -> List[Content]:
     """
     Redirect message to neighbor station via the station bridge
     if neighbor is None, try to broadcast
 
     :param msg:      network message
     :param neighbor: roaming station
     :param bridge:   current station
@@ -422,43 +418,43 @@
     #       we don't need to clone this dictionary to avoid 'neighbor'
     #       be changed to another value before pushing to the bridge.
     # clone = msg.copy_dictionary()
     # msg = ReliableMessage.parse(msg=clone)
     if neighbor is None:
         # broadcast to all neighbor stations
         # except that ones already in msg['recipients']
-        session_push(msg=msg, receiver=bridge)
+        await session_push(msg=msg, receiver=bridge)
         # no need to respond receipt for this broadcast message
         return []
     else:
         assert neighbor != bridge, 'cannot bridge cycled message: %s' % neighbor
         msg['neighbor'] = str(neighbor)
     # push to the bridge
-    if session_push(msg=msg, receiver=bridge) == 0:
+    if await session_push(msg=msg, receiver=bridge) == 0:
         # station bridge not found
         Log.warning(msg='failed to push message to bridge: %s, drop message: %s -> %s'
                         % (bridge, msg.sender, msg.receiver))
         return []
     text = 'Message redirected via station bridge.'
     cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
     cmd['neighbor'] = str(neighbor)
     return [cmd]
 
 
-def session_push(msg: ReliableMessage, receiver: ID) -> int:
+async def session_push(msg: ReliableMessage, receiver: ID) -> int:
     """ push message via active session(s) of receiver """
     success = 0
     center = SessionCenter()
     active_sessions = center.active_sessions(identifier=receiver)
     for session in active_sessions:
-        if session.send_reliable_message(msg=msg):
+        if await session.send_reliable_message(msg=msg):
             success += 1
     return success
 
 
-def get_roaming_station(receiver: ID, database: SessionDBI) -> Optional[ID]:
+async def get_roaming_station(receiver: ID, database: SessionDBI) -> Optional[ID]:
     """ get login command for roaming station """
-    cmd, msg = database.login_command_message(user=receiver)
+    cmd, msg = await database.get_login_command_message(user=receiver)
     if isinstance(cmd, LoginCommand):
         station = cmd.station
         assert isinstance(station, dict), 'login command error: %s' % cmd
         return ID.parse(identifier=station.get('ID'))
```

### Comparing `dimples-0.5.8/dimples/server/messenger.py` & `dimples-1.0.0/dimples/server/messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,67 +41,69 @@
 
 from .dispatcher import Dispatcher
 
 
 class ServerMessenger(CommonMessenger):
 
     # Override
-    def handshake_success(self):
+    async def handshake_success(self):
         session = self.session
         identifier = session.identifier
         remote_address = session.remote_address
         self.warning(msg='user login: %s, socket: %s' % (identifier, remote_address))
         # process suspended messages
-        self._resume_reliable_messages()
+        await self._resume_reliable_messages()
 
-    def _resume_reliable_messages(self):
+    async def _resume_reliable_messages(self):
         packer = self.packer
         assert isinstance(packer, CommonMessagePacker), 'message packer error: %s' % packer
         messages = packer.resume_reliable_messages()
         for msg in messages:
             msg.pop('error', None)
             self.info(msg='processing suspended message: %s -> %s' % (msg.sender, msg.receiver))
             try:
-                responses = self.process_reliable_message(msg=msg)
+                responses = await self.process_reliable_message(msg=msg)
                 for res in responses:
-                    self.send_reliable_message(msg=res, priority=1)
+                    await self.send_reliable_message(msg=res, priority=1)
             except Exception as error:
                 self.error(msg='failed to process incoming message: %s' % error)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         session = self.session
         current = self.facebook.current_user
         sid = current.identifier
         receiver = msg.receiver
         # call super
-        responses = super().process_reliable_message(msg=msg)
+        responses = await super().process_reliable_message(msg=msg)
         # check for first handshake
         if receiver == Station.ANY or msg.group == Station.EVERY:
             # if this message sent to 'station@anywhere', or with group ID 'stations@everywhere',
             # it means the client doesn't have the station's meta (e.g.: first handshaking)
             # or visa maybe expired, here attach them to the first response.
+            meta = await current.meta
+            visa = await current.visa
             for res in responses:
                 if res.sender == sid:
                     # let the first responding message to carry the station's meta & visa
-                    MessageHelper.set_meta(meta=current.meta, msg=res)
-                    MessageHelper.set_visa(visa=current.visa, msg=res)
+                    MessageHelper.set_meta(meta=meta, msg=res)
+                    MessageHelper.set_visa(visa=visa, msg=res)
                     break
         elif session.identifier == sid:
             # station bridge
-            responses = pick_out(messages=responses, bridge=sid)
+            responses = await pick_out(messages=responses, bridge=sid)
         return responses
 
 
-def pick_out(messages: List[ReliableMessage], bridge: ID) -> List[ReliableMessage]:
+async def pick_out(messages: List[ReliableMessage], bridge: ID) -> List[ReliableMessage]:
     responses = []
     dispatcher = Dispatcher()
     for msg in messages:
         receiver = msg.receiver
         if receiver == bridge:
             # respond to the bridge
             responses.append(msg)
         else:
             # this message is not respond to the bridge, the receiver may be
             # roaming to other station, so deliver it via dispatcher here.
-            dispatcher.deliver_message(msg=msg, receiver=receiver)
+            await dispatcher.deliver_message(msg=msg, receiver=receiver)
     return responses
```

### Comparing `dimples-0.5.8/dimples/server/packer.py` & `dimples-1.0.0/dimples/server/packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         if user.type == EntityType.STATION:
             # if it's a roaming message delivered from another neighbor station,
             # shall we trust that neighbor totally and skip verifying too ???
             # TODO: trusted station list
             return True
 
     # Override
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
-        msg = super().deserialize_message(data=data)
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+        msg = await super().deserialize_message(data=data)
         if msg is not None:
             sender = msg.sender
             receiver = msg.receiver
             # check duplicated
             if self.__is_traced(msg=msg):
                 # cycled message
                 if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
@@ -93,22 +93,22 @@
                     # ignore cycled broadcast message
                     self.warning(msg='drop cycled broadcast message: %s -> %s' % (sender, receiver))
                     return None
                 self.warning(msg='cycled message: %s -> %s' % (sender, receiver))
         return msg
 
     # Override
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         # check session ready
         if self.__is_trusted(sender=msg.sender):
             # no need to verify message from this sender
             self.debug(msg='trusted sender: %s' % msg.sender)
             return msg
         # verify after sender is OK
-        return super().verify_message(msg=msg)
+        return await super().verify_message(msg=msg)
 
 
 def get_facebook(packer: CommonMessagePacker) -> CommonFacebook:
     barrack = packer.facebook
     assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
     return barrack
 
@@ -126,27 +126,27 @@
 
     Filters for delivering message
 """
 
 
 class BlockFilter(Logging):
 
-    def is_blocked(self, msg: ReliableMessage) -> bool:
+    async def is_blocked(self, msg: ReliableMessage) -> bool:
         sender = msg.sender
         receiver = msg.receiver
         group = msg.group
         self.debug(msg='checking block-list for: %s -> %s (group: %s)' % (sender, receiver, group))
         # TODO: check block-list
         return False
 
 
 class MuteFilter(Logging):
     """ Filter for Push Notification service """
 
-    def is_muted(self, msg: ReliableMessage) -> bool:
+    async def is_muted(self, msg: ReliableMessage) -> bool:
         sender = msg.sender
         receiver = msg.receiver
         group = msg.group
         self.debug(msg='checking mute-list for: %s -> %s (group: %s)' % (sender, receiver, group))
         if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
             # mute all messages for stations
             return True
```

### Comparing `dimples-0.5.8/dimples/server/processor.py` & `dimples-1.0.0/dimples/server/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,36 +70,36 @@
     def facebook(self) -> CommonFacebook:
         barrack = super().facebook
         assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
         return barrack
 
     # protected
     # noinspection PyMethodMayBeStatic
-    def is_blocked(self, msg: ReliableMessage) -> bool:
+    async def is_blocked(self, msg: ReliableMessage) -> bool:
         block_filter = FilterManager().block_filter
-        return block_filter.is_blocked(msg=msg)
+        return await block_filter.is_blocked(msg=msg)
 
     def _suspend_reliable_message(self, msg: ReliableMessage, error: Dict):
         packer = self.messenger.packer
         assert isinstance(packer, CommonMessagePacker), 'message packer error: %s' % packer
         packer.suspend_reliable_message(msg=msg, error=error)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # check block list
-        if self.is_blocked(msg=msg):
+        if await self.is_blocked(msg=msg):
             self.warning(msg='user is blocked: %s -> %s (group: %s)' % (msg.sender, msg.receiver, msg.group))
             return []
         messenger = self.messenger
         session = messenger.session
         current = self.facebook.current_user
         station = current.identifier
         receiver = msg.receiver
         # 0. verify message
-        s_msg = messenger.verify_message(msg=msg)
+        s_msg = await messenger.verify_message(msg=msg)
         if s_msg is None:
             # TODO: suspend and waiting for sender's meta if not exists
             return []
         # 1. check receiver
         if receiver == station:
             # message to this station
             # maybe a meta command, document command, etc ...
@@ -117,73 +117,73 @@
                 # 1.1. suspend this message for waiting handshake
                 error = {
                     'message': 'user not login',
                 }
                 self._suspend_reliable_message(msg=msg, error=error)
                 # 1.2. ask client to handshake again (with session key)
                 # this message won't be delivered before handshake accepted
-                return self._force_handshake(msg=msg)
+                return await self._force_handshake(msg=msg)
             # session is active and user login success
             # if sender == session.ID,
             #   we can trust this message an no need to verify it;
             # else if sender is a neighbor station,
             #   we can trust it too;
             if receiver == Station.EVERY or receiver == EVERYONE:
                 # broadcast message (to neighbor stations)
                 # e.g.: 'stations@everywhere', 'everyone@everywhere'
-                self._broadcast_message(msg=msg, station=station)
+                await self._broadcast_message(msg=msg, station=station)
                 # if receiver == 'everyone@everywhere':
                 #     broadcast message to all destinations,
                 #     current station is it's receiver too.
             elif receiver.is_broadcast:
                 # broadcast message (to station bots)
                 # e.g.: 'archivist@anywhere', 'announcer@anywhere', 'monitor@anywhere', ...
-                self._broadcast_message(msg=msg, station=station)
+                await self._broadcast_message(msg=msg, station=station)
                 return []
             elif receiver.is_group:
                 # encrypted group messages should be sent to the group assistant,
                 # the station will never process these messages.
-                self._split_group_message(msg=msg, station=station)
+                await self._split_group_message(msg=msg, station=station)
                 return []
             else:
                 # this message is not for current station,
                 # deliver to the real receiver and respond to sender
-                return self._deliver_message(msg=msg)
+                return await self._deliver_message(msg=msg)
         # 2. process message
-        responses = messenger.process_secure_message(msg=s_msg, r_msg=msg)
+        responses = await messenger.process_secure_message(msg=s_msg, r_msg=msg)
         if len(responses) == 0:
             # nothing to respond
             return []
         # 3. sign message
         messages = []
         for res in responses:
-            signed = messenger.sign_message(msg=res)
+            signed = await messenger.sign_message(msg=res)
             if signed is not None:
                 messages.append(signed)
         return messages
         # TODO: override to deliver to the receiver when catch exception "receiver error ..."
 
-    def _force_handshake(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def _force_handshake(self, msg: ReliableMessage) -> List[ReliableMessage]:
         session = self.messenger.session
         sess_id = session.identifier
         current = self.facebook.current_user
         sid = current.identifier
         sender = msg.sender
         if sess_id is not None:
             assert sess_id == sender, 'sender error: %s, %s' % (sender, sess_id)
         # build 'handshake' command message
         command = HandshakeCommand.ask(session=session.key)
         command['force'] = True
-        r_msg = pack_message(content=command, sender=sid, receiver=sender, messenger=self.messenger)
+        r_msg = await pack_message(content=command, sender=sid, receiver=sender, messenger=self.messenger)
         if r_msg is None:
             assert False, 'failed to send "handshake" command to: %s' % sender
         else:
             return [r_msg]
 
-    def _broadcast_message(self, msg: ReliableMessage, station: ID):
+    async def _broadcast_message(self, msg: ReliableMessage, station: ID):
         """ broadcast message to actual recipients """
         sender = msg.sender
         receiver = msg.receiver
         assert receiver.is_broadcast, 'broadcast message error: %s -> %s' % (sender, receiver)
         self.info(msg='broadcast message %s -> %s (%s)' % (sender, receiver, msg.group))
         if receiver.is_user:
             # broadcast message to station bots
@@ -201,45 +201,45 @@
                 self.warning(msg='skip current station: %s -> %s' % (sender, receiver))
                 return False
             else:
                 self.info(msg='forward to bot: %s -> %s' % (name, bot))
                 receiver = bot
         # deliver by dispatcher
         dispatcher = Dispatcher()
-        dispatcher.deliver_message(msg=msg, receiver=receiver)
+        await dispatcher.deliver_message(msg=msg, receiver=receiver)
 
-    def _split_group_message(self, msg: ReliableMessage, station: ID):
+    async def _split_group_message(self, msg: ReliableMessage, station: ID):
         """ redirect group message to assistant """
         sender = msg.sender
         receiver = msg.receiver
         self.error(msg='group message should not send to station: %s, %s -> %s' % (station, sender, receiver))
 
-    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         messenger = self.messenger
         current = self.facebook.current_user
         sid = current.identifier
         sender = msg.sender
         receiver = msg.receiver
         # deliver
         dispatcher = Dispatcher()
-        responses = dispatcher.deliver_message(msg=msg, receiver=receiver)
+        responses = await dispatcher.deliver_message(msg=msg, receiver=receiver)
         assert len(responses) > 0, 'should not happen'
         messages = []
         for res in responses:
-            r_msg = pack_message(content=res, sender=sid, receiver=sender, messenger=messenger)
+            r_msg = await pack_message(content=res, sender=sid, receiver=sender, messenger=messenger)
             if r_msg is None:
                 assert False, 'failed to send respond to: %s' % sender
             else:
                 messages.append(r_msg)
         return messages
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         # 0. process first
-        responses = super().process_content(content=content, r_msg=r_msg)
+        responses = await super().process_content(content=content, r_msg=r_msg)
         messenger = self.messenger
         sender = r_msg.sender
         # 1. check login
         session = messenger.session
         if session.identifier is None:  # or not session.active:
             # not login yet, force to handshake again
             if not isinstance(content, HandshakeCommand):
@@ -268,20 +268,21 @@
         return contents
 
     # Override
     def _create_creator(self) -> ContentProcessorCreator:
         return ServerContentProcessorCreator(facebook=self.facebook, messenger=self.messenger)
 
 
-def pack_message(content: Content, sender: ID, receiver: ID, messenger: CommonMessenger) -> Optional[ReliableMessage]:
+async def pack_message(content: Content, sender: ID, receiver: ID,
+                       messenger: CommonMessenger) -> Optional[ReliableMessage]:
     envelope = Envelope.create(sender=sender, receiver=receiver)
     i_msg = InstantMessage.create(head=envelope, body=content)
-    s_msg = messenger.encrypt_message(msg=i_msg)
+    s_msg = await messenger.encrypt_message(msg=i_msg)
     if s_msg is not None:
-        return messenger.sign_message(msg=s_msg)
+        return await messenger.sign_message(msg=s_msg)
 
 
 class ServerContentProcessorCreator(BaseContentProcessorCreator):
 
     # Override
     def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
         # default
```

### Comparing `dimples-0.5.8/dimples/server/push.py` & `dimples-1.0.0/dimples/server/push.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import threading
 import time
 from abc import ABC, abstractmethod
 from typing import Optional, List, Dict
 
 from dimsdk import ID, ReliableMessage
 
-from ..utils import Runner, Daemon
+from ..utils import Runner, DaemonRunner
 from ..utils import Singleton, Logging
 
 
 class MessageQueue(Logging):
 
     def __init__(self):
         super().__init__()
@@ -107,30 +107,28 @@
         with self.__lock:
             self.__badges.pop(identifier, None)
 
 
 class PushService(ABC):
 
     @abstractmethod
-    def process(self, messages: List[ReliableMessage]) -> bool:
+    async def process(self, messages: List[ReliableMessage]) -> bool:
         """ build and push notification for a batch of messages """
         raise NotImplemented
 
 
 @Singleton
-class PushCenter(Runner, Logging):
+class PushCenter(DaemonRunner, Logging):
 
     def __init__(self):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__queue = MessageQueue()
         self.__keeper = BadgeKeeper()
         self.__service: Optional[PushService] = None
-        # background thread
-        self.__daemon = Daemon(target=self)
-        self.__daemon.start()
+        Runner.async_run(coroutine=self.start())
 
     @property
     def service(self) -> Optional[PushService]:
         return self.__service
 
     @service.setter
     def service(self, pusher: PushService):
@@ -147,21 +145,21 @@
 
     def push_notification(self, msg: ReliableMessage):
         """ Push notification for msg receiver """
         queue = self.__queue
         queue.add_message(msg=msg)
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         # 1. get waiting messages
         queue = self.__queue
         messages = queue.get_messages()
         if messages is None:
             # nothing to do now, return False to have a rest
             return False
         # 2. get message processor
         service = self.__service
         if service is None:
             self.error(msg='push service not found')
             return False
         # 3. process
-        return service.process(messages=messages)
+        return await service.process(messages=messages)
```

### Comparing `dimples-0.5.8/dimples/server/session.py` & `dimples-1.0.0/dimples/server/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,25 +32,26 @@
     Session Server
     ~~~~~~~~~~~~~~
 
     for login user
 """
 
 import socket
-import threading
 import traceback
+import weakref
 from typing import Optional, List, Tuple
 
 from dimsdk import ID, EntityType
 from dimsdk import ReliableMessage
 
 from startrek import Docker, DockerStatus
 from startrek import Arrival, Departure
+from startrek.net.channel import is_closed
 
-from ..utils import Log
+from ..utils import Log, Runner
 from ..utils import hex_encode, random_bytes
 from ..utils import get_msg_sig, get_msg_info
 from ..common import SessionDBI, MessageDBI, ReliableMessageDBI
 from ..conn import MessageWrapper
 from ..conn import BaseSession
 from ..conn import WSArrival, MarsStreamArrival, MTPStreamArrival
 
@@ -80,77 +81,78 @@
                 After received 'offline' command, it will be set to False;
                 and when received 'online' it will be True again.
                 Only push message when it's True.
     """
 
     def __init__(self, remote: Tuple[str, int], sock: socket.socket, database: SessionDBI):
         super().__init__(remote=remote, sock=sock, database=database)
+        self.__sock = weakref.ref(sock)
         self.__key = generate_session_key()
 
     @property
     def key(self) -> str:
         return self.__key
 
-    def __load_cached_messages(self):
-        if self.identifier is None or not self.active:
-            return False
-        # load cached message asynchronously
-        threading.Thread(target=load_cached_messages, args=(self,)).start()
-        # load_cached_messages(session=self)
-        return True
-
     # Override
     def set_identifier(self, identifier: ID) -> bool:
         old = self.identifier
         if super().set_identifier(identifier=identifier):
             session_change_id(session=self, new_id=identifier, old_id=old)
-            self.__load_cached_messages()
+            # load cached message asynchronously
+            Runner.async_run(coroutine=load_cached_messages(session=self))
             return True
 
     # Override
     def set_active(self, active: bool, when: float = None) -> bool:
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
-            if active:
-                self.__load_cached_messages()
+            # load cached message asynchronously
+            Runner.async_run(coroutine=load_cached_messages(session=self))
             return True
 
     @property  # Override
     def running(self) -> bool:
         if super().running:
-            gate = self.gate
-            conn = gate.get_channel(remote=self.remote_address, local=None)
-            return not (conn is None or conn.closed)
+            # gate = self.gate
+            # conn = gate.get_channel(remote=self.remote_address, local=None)
+            # return not (conn is None or conn.closed)
+            sock = self.__sock()
+            return not (sock is None or is_closed(sock=sock))
+
+    # Override
+    async def start(self):
+        await super().start()
+        await self.run()
 
     #
     #   Docker Delegate
     #
 
     # Override
-    def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
+    async def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
         # super().docker_status_changed(previous=previous, current=current, docker=docker)
         if current is None or current == DockerStatus.ERROR:
             # connection error or session finished
             self.set_active(active=False)
-            self.stop()
+            await self.stop()
         elif current == DockerStatus.READY:
             # connected/reconnected
             self.set_active(active=True)
 
     # Override
-    def docker_received(self, ship: Arrival, docker: Docker):
+    async def docker_received(self, ship: Arrival, docker: Docker):
         # super().docker_received(ship=ship, docker=docker)
         all_responses = []
         messenger = self.messenger
         # 1. get data packages from arrival ship's payload
         packages = get_data_packages(ship=ship)
         for pack in packages:
             try:
                 # 2. process each data package
-                responses = messenger.process_package(data=pack)
+                responses = await messenger.process_package(data=pack)
                 for res in responses:
                     if len(res) == 0:
                         # should not happen
                         continue
                     all_responses.append(res)
             except Exception as error:
                 source = docker.remote_address
@@ -161,28 +163,28 @@
         gate = self.gate
         source = docker.remote_address
         destination = docker.local_address
         # 3. send responses
         if len(all_responses) > 0:
             # respond separately
             for res in all_responses:
-                gate.send_response(payload=res, ship=ship, remote=source, local=destination)
+                await gate.send_response(payload=res, ship=ship, remote=source, local=destination)
         elif isinstance(ship, MarsStreamArrival):
             # station MUST respond something to client request (Tencent Mars)
-            gate.send_response(payload=b'', ship=ship, remote=source, local=destination)
+            await gate.send_response(payload=b'', ship=ship, remote=source, local=destination)
 
     # Override
-    def docker_sent(self, ship: Departure, docker: Docker):
+    async def docker_sent(self, ship: Departure, docker: Docker):
         if isinstance(ship, MessageWrapper):
             msg = ship.msg
             if msg is not None:
                 # remove from database for actual receiver
                 receiver = self.identifier
                 db = self.messenger.database
-                remove_reliable_message(msg=msg, receiver=receiver, database=db)
+                await remove_reliable_message(msg=msg, receiver=receiver, database=db)
 
 
 def get_data_packages(ship: Arrival) -> List[bytes]:
     # get payload
     if isinstance(ship, MTPStreamArrival):
         payload = ship.payload
     elif isinstance(ship, MarsStreamArrival):
@@ -218,31 +220,32 @@
     elif active:
         # user online, clear badges
         center = PushCenter()
         center.reset_badge(identifier=identifier)
         return True
 
 
-def load_cached_messages(session: ServerSession):
+async def load_cached_messages(session: ServerSession):
     identifier = session.identifier
-    assert identifier is not None and session.active, 'session error: %s' % identifier
+    if identifier is None or not session.active:
+        return False
     messenger = session.messenger
     db = messenger.database
     limit = ReliableMessageDBI.CACHE_LIMIT
-    messages = db.reliable_messages(receiver=identifier, limit=limit)
+    messages = await db.get_reliable_messages(receiver=identifier, limit=limit)
     cnt = len(messages)
     Log.info(msg='[DB] %d cached message(s) loaded for: %s' % (cnt, identifier))
     for msg in messages:
-        data = messenger.serialize_message(msg=msg)
-        ok = session.queue_message_package(msg=msg, data=data, priority=1)
+        data = await messenger.serialize_message(msg=msg)
+        ok = await session.queue_message_package(msg=msg, data=data, priority=1)
         sig = get_msg_sig(msg=msg)
         Log.info(msg='queue message for: %s, %s, %s' % (identifier, ok, sig))
 
 
-def remove_reliable_message(msg: ReliableMessage, receiver: ID, database: MessageDBI):
+async def remove_reliable_message(msg: ReliableMessage, receiver: ID, database: MessageDBI):
     # 0. if session ID is empty, means user not login;
     #    this message must be a handshake command, and
     #    its receiver must be the targeted user.
     # 1. if this session is a station, check original receiver;
     #    a message to station won't be stored.
     # 2. if the msg.receiver is a different user ID, means it's
     #    a roaming message, remove it for actual receiver.
@@ -252,8 +255,8 @@
         # if msg.receiver == receiver:
         #     # station message won't be stored
         #     return False
         receiver = msg.receiver
     info = get_msg_info(msg=msg)
     Log.info(msg='message sent for %s, remove from db: %s' % (receiver, info))
     # remove sent message from database
-    return database.remove_reliable_message(msg=msg, receiver=receiver)
+    return await database.remove_reliable_message(msg=msg, receiver=receiver)
```

### Comparing `dimples-0.5.8/dimples/server/session_center.py` & `dimples-1.0.0/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/server/trace.py` & `dimples-1.0.0/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/station/__init__.py` & `dimples-1.0.0/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/station/shared.py` & `dimples-1.0.0/dimples/station/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         sys.exit(0)
     # load config from file
     config = Config.load(file=ini_file)
     print('>>> config loaded: %s => %s' % (ini_file, config))
     return config
 
 
-def create_database(config: Config) -> Tuple[AccountDBI, MessageDBI, SessionDBI]:
+async def create_database(config: Config) -> Tuple[AccountDBI, MessageDBI, SessionDBI]:
     """ Step 2: create database """
     root = config.database_root
     public = config.database_public
     private = config.database_private
     # create database
     adb = AccountDatabase(root=root, public=public, private=private)
     mdb = MessageDatabase(root=root, public=public, private=private)
@@ -119,43 +119,43 @@
     sdb.show_info()
     # default provider
     provider = ProviderInfo.GSP
     # add neighbors
     neighbors = config.neighbors
     for node in neighbors:
         print('adding neighbor node: %s' % node)
-        sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
+        await sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
     return adb, mdb, sdb
 
 
-def create_facebook(database: AccountDBI, current_user: ID) -> CommonFacebook:
+async def create_facebook(database: AccountDBI, current_user: ID) -> CommonFacebook:
     """ Step 3: create facebook """
     facebook = CommonFacebook()
     # create archivist for facebook
     shared = GlobalVariable()
     shared.messenger = create_messenger(facebook=facebook, database=shared.mdb, session=None)
     archivist = ServerArchivist(database=database)
     archivist.messenger = shared.messenger
     archivist.facebook = facebook
     facebook.archivist = archivist
     # make sure private keys exists
-    sign_key = facebook.private_key_for_visa_signature(identifier=current_user)
-    msg_keys = facebook.private_keys_for_decryption(identifier=current_user)
+    sign_key = await facebook.private_key_for_visa_signature(identifier=current_user)
+    msg_keys = await facebook.private_keys_for_decryption(identifier=current_user)
     assert sign_key is not None, 'failed to get sign key for current user: %s' % current_user
     assert len(msg_keys) > 0, 'failed to get msg keys: %s' % current_user
     print('set current user: %s' % current_user)
-    user = facebook.user(identifier=current_user)
+    user = await facebook.get_user(identifier=current_user)
     assert user is not None, 'failed to get current user: %s' % current_user
-    visa = user.visa
+    visa = await user.visa
     if visa is not None:
         # refresh visa
         now = time.time()
         visa.set_property(key='time', value=now)
         visa.sign(private_key=sign_key)
-        facebook.save_document(document=visa)
+        await facebook.save_document(document=visa)
     facebook.current_user = user
     return facebook
 
 
 def create_messenger(facebook: CommonFacebook, database: MessageDBI,
                      session: Optional[ServerSession]) -> ServerMessenger:
     # 1. create messenger with session and MessageDB
```

### Comparing `dimples-0.5.8/dimples/station/start.py` & `dimples-1.0.0/dimples/station/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,25 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-
 import os
 import sys
 from socketserver import ThreadingTCPServer
 
 path = os.path.abspath(__file__)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 sys.path.insert(0, path)
 
-from dimples.utils import Log
+from dimples.utils import Log, Runner
 
 from dimples.station.shared import GlobalVariable
 from dimples.station.shared import create_config, create_database, create_facebook
 from dimples.station.shared import create_dispatcher
 from dimples.station.shared import create_ans
 from dimples.station.handler import RequestHandler
 
@@ -54,29 +53,29 @@
 #
 Log.LEVEL = Log.DEVELOP
 
 
 DEFAULT_CONFIG = '/etc/dim/station.ini'
 
 
-def main():
+async def main():
     # create global variable
     shared = GlobalVariable()
     # Step 1: load config
     config = create_config(app_name='DIM Network Station', default_config=DEFAULT_CONFIG)
     shared.config = config
     # Step 2: create database
-    adb, mdb, sdb = create_database(config=config)
+    adb, mdb, sdb = await create_database(config=config)
     shared.adb = adb
     shared.mdb = mdb
     shared.sdb = sdb
     # Step 3: create facebook
     sid = config.station_id
     assert sid is not None, 'current station ID not set: %s' % config
-    facebook = create_facebook(database=adb, current_user=sid)
+    facebook = await create_facebook(database=adb, current_user=sid)
     shared.facebook = facebook
     # Step 4: create dispatcher
     create_dispatcher(shared=shared)
     # Step 5: create ANS
     create_ans(config=config)
     # check bind host & port
     host = config.station_host
@@ -99,8 +98,8 @@
     except KeyboardInterrupt as ex:
         Log.info(msg='~~~~~~~~ %s' % ex)
     finally:
         Log.info(msg='======== station shutdown!')
 
 
 if __name__ == '__main__':
-    main()
+    Runner.sync_run(main=main())
```

### Comparing `dimples-0.5.8/dimples/utils/__init__.py` & `dimples-1.0.0/dimples/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from dimsdk import Converter
 from dimsdk import DateTime
 from dimsdk import ReliableMessage
 from dimsdk import DocumentHelper
 
 from dimplugins.crypto.aes import random_bytes
 
-from startrek.fsm import Runnable, Runner, Daemon
+from startrek.fsm import Runnable, Runner, Daemon, DaemonRunner
 from startrek.fsm import Delegate as StateDelegate
 from startrek.net.channel import get_remote_address, get_local_address
 
 
 from .singleton import Singleton
 from .log import Log, Logging
 from .dos import Path, File, TextFile, JSONFile
@@ -118,15 +118,15 @@
     'utf8_encode', 'utf8_decode',
     'json_encode', 'json_decode',
 
     'random_bytes',
 
     'Converter',
 
-    'Runnable', 'Runner', 'Daemon',
+    'Runnable', 'Runner', 'Daemon', 'DaemonRunner',
     'StateDelegate',
 
     'get_remote_address', 'get_local_address',
 
 
     'Singleton',
     'Log', 'Logging',
```

### Comparing `dimples-0.5.8/dimples/utils/cache.py` & `dimples-1.0.0/dimples/utils/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 
 """
     Database module
     ~~~~~~~~~~~~~~~
 
 """
 
-import time
 from typing import TypeVar, Generic, Optional, Dict, Set, Tuple
 
-from startrek.fsm import Daemon, Runnable
+from startrek.fsm import Runnable, Runner, Daemon
 from dimsdk import DateTime
 
 from .singleton import Singleton
 
 
 K = TypeVar('K')
 V = TypeVar('V')
@@ -136,36 +135,38 @@
 
 @Singleton
 class CacheManager(Runnable):
 
     def __init__(self):
         self.__pools: Dict[str, CachePool] = {}  # name -> pool
         # thread for cleaning caches
+        self.__running = True
         self.__daemon = Daemon(target=self)
-        self.__running = False
+        self.__daemon.start()
 
     @property
     def running(self) -> bool:
         return self.__running
 
-    def start(self):
-        self.__running = True
-        self.__daemon.start()
-
-    def stop(self):
+    async def stop(self):
+        # 1. mark this gate to stopped
+        self.__running = False
+        # 2. waiting for the gate to stop
+        await Runner.sleep(seconds=5)
+        # 3. cancel the async task
         self.__daemon.stop()
 
     # Override
-    def run(self):
+    async def run(self):
         next_time = 0
         while self.running:
             # try to purge each 5 minutes
             now = DateTime.now()
             if now < next_time:
-                time.sleep(2)
+                await Runner.sleep(seconds=2)
                 continue
             else:
                 next_time = DateTime(now.timestamp + 300)
             try:
                 count = self.purge(now=now)
                 print('[MEM] purge %d item(s) from cache pools' % count)
             except Exception as error:
```

### Comparing `dimples-0.5.8/dimples/utils/config.py` & `dimples-1.0.0/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/utils/dos.py` & `dimples-1.0.0/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/utils/log.py` & `dimples-1.0.0/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples/utils/singleton.py` & `dimples-1.0.0/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.8/dimples.egg-info/PKG-INFO` & `dimples-1.0.0/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.8
+Version: 1.0.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.8/dimples.egg-info/SOURCES.txt` & `dimples-1.0.0/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

