# Comparing `tmp/ANX-0.7.7.tar.gz` & `tmp/ANX-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.7.7.tar", last modified: Thu Apr 25 09:28:45 2024, max compression
+gzip compressed data, was "ANX-0.7.8.tar", last modified: Fri May 10 21:13:11 2024, max compression
```

## Comparing `ANX-0.7.7.tar` & `ANX-0.7.8.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.643238 ANX-0.7.7/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.597814 ANX-0.7.7/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-25 09:28:45.000000 ANX-0.7.7/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4882 2024-04-25 09:28:45.000000 ANX-0.7.7/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-25 09:28:45.000000 ANX-0.7.7/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-25 09:28:45.000000 ANX-0.7.7/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-25 09:28:45.000000 ANX-0.7.7/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.605932 ANX-0.7.7/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    34820 2024-04-25 09:25:31.000000 ANX-0.7.7/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.606533 ANX-0.7.7/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     4025 2024-04-12 06:25:09.000000 ANX-0.7.7/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.610907 ANX-0.7.7/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.7/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.7/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.7/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.7/AndroidQQ/http/cip.py
--rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.7/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     4734 2024-04-11 04:47:50.000000 ANX-0.7.7/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.7.7/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.7.7/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.7/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.7/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.611190 ANX-0.7.7/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.611297 ANX-0.7.7/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.611672 ANX-0.7.7/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.612265 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.613455 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.613970 ANX-0.7.7/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.614518 ANX-0.7.7/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.615442 ANX-0.7.7/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.616016 ANX-0.7.7/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.617010 ANX-0.7.7/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.617348 ANX-0.7.7/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.621568 ANX-0.7.7/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.623658 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.624614 ANX-0.7.7/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.7/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.7/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.625278 ANX-0.7.7/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.7/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.7/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.628124 ANX-0.7.7/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.629608 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.630119 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.633566 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.635753 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.638247 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.638533 ANX-0.7.7/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.639553 ANX-0.7.7/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.7/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.640509 ANX-0.7.7/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.641013 ANX-0.7.7/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.641286 ANX-0.7.7/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.641596 ANX-0.7.7/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.7/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.641983 ANX-0.7.7/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.7/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.642700 ANX-0.7.7/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.642830 ANX-0.7.7/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-25 09:28:45.642958 ANX-0.7.7/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.7/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-25 09:28:45.643109 ANX-0.7.7/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.7/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-25 09:28:45.643292 ANX-0.7.7/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      601 2024-04-25 09:28:36.000000 ANX-0.7.7/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.335695 ANX-0.7.8/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.297981 ANX-0.7.8/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-10 21:13:11.000000 ANX-0.7.8/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4882 2024-05-10 21:13:11.000000 ANX-0.7.8/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-05-10 21:13:11.000000 ANX-0.7.8/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-05-10 21:13:11.000000 ANX-0.7.8/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-05-10 21:13:11.000000 ANX-0.7.8/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.299017 ANX-0.7.8/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    34781 2024-05-10 20:44:20.000000 ANX-0.7.8/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.299382 ANX-0.7.8/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     4299 2024-05-08 06:01:05.000000 ANX-0.7.8/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.302579 ANX-0.7.8/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.8/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.8/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.8/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.8/AndroidQQ/http/cip.py
+-rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.8/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     4734 2024-04-11 04:47:50.000000 ANX-0.7.8/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.7.8/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.7.8/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.8/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.8/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.302951 ANX-0.7.8/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.303050 ANX-0.7.8/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.303496 ANX-0.7.8/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.304125 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.305510 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.306068 ANX-0.7.8/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.306593 ANX-0.7.8/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.307094 ANX-0.7.8/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.307567 ANX-0.7.8/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.308484 ANX-0.7.8/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.308745 ANX-0.7.8/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.312697 ANX-0.7.8/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.314933 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.315698 ANX-0.7.8/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.8/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.8/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.316520 ANX-0.7.8/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.8/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.8/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.319064 ANX-0.7.8/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.322118 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.322621 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.325973 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.328195 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.330612 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.330896 ANX-0.7.8/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1043 2024-05-10 20:44:20.000000 ANX-0.7.8/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.331572 ANX-0.7.8/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.8/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.332255 ANX-0.7.8/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.332870 ANX-0.7.8/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.333101 ANX-0.7.8/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.333398 ANX-0.7.8/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.8/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.333792 ANX-0.7.8/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.8/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.334869 ANX-0.7.8/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.335046 ANX-0.7.8/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-10 21:13:11.335216 ANX-0.7.8/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.8/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-10 21:13:11.335474 ANX-0.7.8/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.8/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-05-10 21:13:11.335742 ANX-0.7.8/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      601 2024-05-10 21:13:10.000000 ANX-0.7.8/setup.py
```

### Comparing `ANX-0.7.7/ANX.egg-info/SOURCES.txt` & `ANX-0.7.8/ANX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/Android.py` & `ANX-0.7.8/AndroidQQ/Android.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,24 +420,23 @@
                 iGetDevListType=iGetDevListType
 
             )
             return GetDevLoginInfo_profile(info, item)
 
         return self.tcp_task(req_func, GetDevLoginInfo_res)
 
-    def del_login_info(self, **kwargs):
+    def del_login_info(self, key):
         """删除登录信息
         key= 获取设备信息返回
         """
 
-        data = StatSvc.DelDevLoginInfo(self.info, **kwargs)
-        data = self.Tcp_send(data)
-        if data:
-            data = StatSvc.DelDevLoginInfo_res(data)
-        return data
+        def req_func(info):
+            return StatSvc.DelDevLoginInfo(info, key)
+
+        return self.tcp_task(req_func, StatSvc.DelDevLoginInfo_res)
 
     def avatar_test_(self, **kwargs):
         """
         测试
         """
 
         data = avatar_test(self.info)
```

### Comparing `ANX-0.7.7/AndroidQQ/Tcp.py` & `ANX-0.7.8/AndroidQQ/Tcp.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,20 @@
                 if data:
                     repackage(data, client)
                 else:
                     disconnect_client(client)
             except ConnectionResetError as e:
                 log.error(f"连接重置错误: {e}")
                 disconnect_client(client)
+            except OSError as e:
+                if e.errno == 9:  # Bad file descriptor
+                    log.error(f"尝试操作已关闭的套接字: {e}")
+                else:
+                    log.error(f"OS错误: {e}")
+                disconnect_client(client)
 
             # if not data:
             #     disconnect_client(client, clients, client_info)
             #     log.info('断开连接')
             # else:
             #     # log.info(f"从客户端收到的数据: {data.hex()}")
             #     repackage(data, client)
```

### Comparing `ANX-0.7.7/AndroidQQ/http/ClientKey.py` & `ANX-0.7.8/AndroidQQ/http/ClientKey.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/accounts.py` & `ANX-0.7.8/AndroidQQ/http/accounts.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/cip.py` & `ANX-0.7.8/AndroidQQ/http/cip.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/friends.py` & `ANX-0.7.8/AndroidQQ/http/friends.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/game_credit.py` & `ANX-0.7.8/AndroidQQ/http/game_credit.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/level.py` & `ANX-0.7.8/AndroidQQ/http/level.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/music.py` & `ANX-0.7.8/AndroidQQ/http/music.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/qqsignin.py` & `ANX-0.7.8/AndroidQQ/http/qqsignin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/http/weishi.py` & `ANX-0.7.8/AndroidQQ/http/weishi.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.7.8/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.7.8/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.7.8/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.7.8/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.7.8/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.7.8/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.7.8/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.8/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/friendlist.py` & `ANX-0.7.8/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/test.py` & `ANX-0.7.8/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.7.8/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.7.8/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.7.8/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.7.8/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/MessageSvc.py` & `ANX-0.7.8/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.7.8/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/OidbSvc.py` & `ANX-0.7.8/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.7.8/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.7.8/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.7.8/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/StatSvc.py` & `ANX-0.7.8/AndroidQQ/struct/StatSvc.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 import zlib
 
 from Jce import JceInputStream, JceStruct
 
 from AndroidQQ.struct.head import *
 
 
-def DelDevLoginInfo(info, **kwargs):
+def DelDevLoginInfo(info, key):
     """删除登录信息"""
-    key = kwargs.get('key', b'')
-    if isinstance(key, str):
-        key = bytes.fromhex(key)
-
+    key = bytes.fromhex(key)
     _data = JceWriter().write_bytes(key, 0)
 
     jce = JceWriter()
     jce.write_bytes(info.Guid, 0)
     jce.write_string('com.tencent.mobileqq', 1)
     jce.write_jce_struct_list([_data], 2)
     jce.write_int32(1, 3)
```

### Comparing `ANX-0.7.7/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.8/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Tlv.py` & `ANX-0.7.8/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/Tlv_res.py` & `ANX-0.7.8/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.7.8/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.7.8/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.7.8/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/head.py` & `ANX-0.7.8/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.7.8/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.7.8/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/struct/wtlogin.py` & `ANX-0.7.8/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/utils/build_device.py` & `ANX-0.7.8/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/utils/ecdh.py` & `ANX-0.7.8/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/utils/sso_server.py` & `ANX-0.7.8/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/AndroidQQ/utils/tool.py` & `ANX-0.7.8/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.7/setup.py` & `ANX-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.7.7',
+    version='0.7.8',
     url='https://github.com/grayrail000/AndroidQQ',
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
```

