# Comparing `tmp/copyparty-1.9.8.tar.gz` & `tmp/copyparty-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.9.8.tar", last modified: Fri Oct  6 18:12:11 2023, max compression
+gzip compressed data, was "copyparty-1.9.9.tar", last modified: Sat Oct  7 22:46:29 2023, max compression
```

## Comparing `copyparty-1.9.8.tar` & `copyparty-1.9.9.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.953505 copyparty-1.9.8/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.9.8/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)   104183 2023-10-06 18:12:11.952504 copyparty-1.9.8/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)   101880 2023-10-06 13:00:15.000000 copyparty-1.9.8/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.938505 copyparty-1.9.8/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    81729 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      253 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    71161 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.940505 copyparty-1.9.8/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3916 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7239 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/cert.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7685 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15369 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   135664 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16044 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17469 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6220 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/metrics.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16891 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    12285 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/multicast.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/pwhash.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.940505 copyparty-1.9.8/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/res/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.9.8/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    13967 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6343 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3771 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.940505 copyparty-1.9.8/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.941505 copyparty-1.9.8/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.942505 copyparty-1.9.8/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2962 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    26150 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8520 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17169 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3852 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10677 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   127182 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    73532 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.946504 copyparty-1.9.8/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.947505 copyparty-1.9.8/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    36595 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/web/a/u2c.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.9.8/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7379 2023-09-29 13:11:17.000000 copyparty-1.9.8/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    11127 2023-09-30 22:48:57.000000 copyparty-1.9.8/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5426 2023-09-29 14:27:36.000000 copyparty-1.9.8/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    61939 2023-09-30 22:48:30.000000 copyparty-1.9.8/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.9.8/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      588 2023-08-15 14:05:51.000000 copyparty-1.9.8/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.9.8/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.947505 copyparty-1.9.8/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.9.8/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.9.8/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.9.8/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.9.8/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:53.000000 copyparty-1.9.8/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.951505 copyparty-1.9.8/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-06 18:11:54.000000 copyparty-1.9.8/copyparty/web/deps/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22291 2023-08-26 17:38:50.000000 copyparty-1.9.8/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      572 2023-04-01 14:48:09.000000 copyparty-1.9.8/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.9.8/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1468 2022-12-29 03:41:18.000000 copyparty-1.9.8/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.9.8/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1637 2022-12-29 03:41:18.000000 copyparty-1.9.8/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.9.8/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7033 2023-04-01 14:23:12.000000 copyparty-1.9.8/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8107 2021-07-22 23:48:12.000000 copyparty-1.9.8/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.9.8/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4074 2023-09-17 12:03:19.000000 copyparty-1.9.8/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4244 2023-09-20 22:42:58.000000 copyparty-1.9.8/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.9.8/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8251 2023-09-17 11:07:31.000000 copyparty-1.9.8/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.9.8/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2023-08-26 17:23:29.000000 copyparty-1.9.8/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.9.8/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.9.8/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      894 2023-09-20 22:07:14.000000 copyparty-1.9.8/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.9.8/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3746 2023-09-29 14:28:23.000000 copyparty-1.9.8/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1255 2023-09-30 14:36:14.000000 copyparty-1.9.8/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10591 2023-09-29 14:28:31.000000 copyparty-1.9.8/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.9.8/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2441 2023-09-03 19:48:14.000000 copyparty-1.9.8/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21729 2023-09-23 11:18:06.000000 copyparty-1.9.8/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    13709 2023-09-29 13:52:32.000000 copyparty-1.9.8/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.9.8/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-06 18:12:11.939504 copyparty-1.9.8/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)   104183 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2782 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-10-06 18:12:11.000000 copyparty-1.9.8/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-09-01 21:13:21.000000 copyparty-1.9.8/pyproject.toml
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-10-06 18:12:11.953505 copyparty-1.9.8/setup.cfg
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.398264 copyparty-1.9.9/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.9.9/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)   104183 2023-10-07 22:46:29.398264 copyparty-1.9.9/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)   101880 2023-10-06 13:00:15.000000 copyparty-1.9.9/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.386264 copyparty-1.9.9/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    81730 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      253 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    71161 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.388264 copyparty-1.9.9/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3916 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7239 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/cert.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7891 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15369 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   135664 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16044 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17469 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6220 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/metrics.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16891 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    12285 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/multicast.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/pwhash.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.388264 copyparty-1.9.9/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/res/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.9.9/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    13967 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6343 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3771 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.388264 copyparty-1.9.9/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.389263 copyparty-1.9.9/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.390264 copyparty-1.9.9/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2962 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    26150 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8520 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17169 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3852 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10677 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   128349 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    73532 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.393264 copyparty-1.9.9/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.394264 copyparty-1.9.9/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    36595 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/web/a/u2c.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.9.9/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7379 2023-09-29 13:11:17.000000 copyparty-1.9.9/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    11127 2023-09-30 22:48:57.000000 copyparty-1.9.9/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5426 2023-09-29 14:27:36.000000 copyparty-1.9.9/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    61939 2023-09-30 22:48:30.000000 copyparty-1.9.9/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.9.9/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      588 2023-08-15 14:05:51.000000 copyparty-1.9.9/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.9.9/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.394264 copyparty-1.9.9/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.9.9/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.9.9/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.9.9/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.9.9/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.397264 copyparty-1.9.9/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:11.000000 copyparty-1.9.9/copyparty/web/deps/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22291 2023-08-26 17:38:50.000000 copyparty-1.9.9/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      572 2023-04-01 14:48:09.000000 copyparty-1.9.9/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.9.9/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1468 2022-12-29 03:41:18.000000 copyparty-1.9.9/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.9.9/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1637 2022-12-29 03:41:18.000000 copyparty-1.9.9/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.9.9/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7033 2023-04-01 14:23:12.000000 copyparty-1.9.9/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8107 2021-07-22 23:48:12.000000 copyparty-1.9.9/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.9.9/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4074 2023-09-17 12:03:19.000000 copyparty-1.9.9/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4244 2023-09-20 22:42:58.000000 copyparty-1.9.9/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.9.9/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8251 2023-09-17 11:07:31.000000 copyparty-1.9.9/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.9.9/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2023-08-26 17:23:29.000000 copyparty-1.9.9/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.9.9/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.9.9/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      894 2023-09-20 22:07:14.000000 copyparty-1.9.9/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.9.9/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3746 2023-09-29 14:28:23.000000 copyparty-1.9.9/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1255 2023-09-30 14:36:14.000000 copyparty-1.9.9/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10591 2023-09-29 14:28:31.000000 copyparty-1.9.9/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.9.9/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2441 2023-09-03 19:48:14.000000 copyparty-1.9.9/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21729 2023-09-23 11:18:06.000000 copyparty-1.9.9/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    13709 2023-09-29 13:52:32.000000 copyparty-1.9.9/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.9.9/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-07 22:46:29.387264 copyparty-1.9.9/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)   104183 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2782 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-10-07 22:46:29.000000 copyparty-1.9.9/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-09-01 21:13:21.000000 copyparty-1.9.9/pyproject.toml
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-10-07 22:46:29.398264 copyparty-1.9.9/setup.cfg
```

### Comparing `copyparty-1.9.8/LICENSE` & `copyparty-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/PKG-INFO` & `copyparty-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.9.8
+Version: 1.9.9
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.9.8/README.md` & `copyparty-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/__init__.py` & `copyparty-1.9.9/copyparty/__init__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/__main__.py` & `copyparty-1.9.9/copyparty/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,15 +793,15 @@
     ap2.add_argument("--unpost", metavar="SEC", type=int, default=3600*12, help="grace period where uploads can be deleted by the uploader, even without delete permissions; 0=disabled")
     ap2.add_argument("--blank-wt", metavar="SEC", type=int, default=300, help="file write grace period (any client can write to a blank file last-modified more recently than SEC seconds ago)")
     ap2.add_argument("--reg-cap", metavar="N", type=int, default=38400, help="max number of uploads to keep in memory when running without -e2d; roughly 1 MiB RAM per 600")
     ap2.add_argument("--no-fpool", action="store_true", help="disable file-handle pooling -- instead, repeatedly close and reopen files during upload (very slow on windows)")
     ap2.add_argument("--use-fpool", action="store_true", help="force file-handle pooling, even when it might be dangerous (multiprocessing, filesystems lacking sparse-files support, ...)")
     ap2.add_argument("--hardlink", action="store_true", help="prefer hardlinks instead of symlinks when possible (within same filesystem) (volflag=hardlink)")
     ap2.add_argument("--never-symlink", action="store_true", help="do not fallback to symlinks when a hardlink cannot be made (volflag=neversymlink)")
-    ap2.add_argument("--no-dedup", action="store_true", help="disable symlink/hardlink creation; copy file contents instead (volflag=copydupes")
+    ap2.add_argument("--no-dedup", action="store_true", help="disable symlink/hardlink creation; copy file contents instead (volflag=copydupes)")
     ap2.add_argument("--no-dupe", action="store_true", help="reject duplicate files during upload; only matches within the same volume (volflag=nodupe)")
     ap2.add_argument("--no-snap", action="store_true", help="disable snapshots -- forget unfinished uploads on shutdown; don't create .hist/up2k.snap files -- abandoned/interrupted uploads must be cleaned up manually")
     ap2.add_argument("--rand", action="store_true", help="force randomized filenames, --nrand chars long (volflag=rand)")
     ap2.add_argument("--nrand", metavar="NUM", type=int, default=9, help="randomized filenames length (volflag=nrand)")
     ap2.add_argument("--magic", action="store_true", help="enable filetype detection on nameless uploads (volflag=magic)")
     ap2.add_argument("--df", metavar="GiB", type=float, default=0, help="ensure GiB free disk space by rejecting upload requests")
     ap2.add_argument("--sparse", metavar="MiB", type=int, default=4, help="windows-only: minimum size of incoming uploads through up2k before they are made into sparse files")
```

### Comparing `copyparty-1.9.8/copyparty/authsrv.py` & `copyparty-1.9.9/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/bos/bos.py` & `copyparty-1.9.9/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/bos/path.py` & `copyparty-1.9.9/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/broker_mp.py` & `copyparty-1.9.9/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/broker_mpw.py` & `copyparty-1.9.9/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/broker_thr.py` & `copyparty-1.9.9/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/broker_util.py` & `copyparty-1.9.9/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/cert.py` & `copyparty-1.9.9/copyparty/cert.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/cfg.py` & `copyparty-1.9.9/copyparty/cfg.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,15 +158,16 @@
         "sb_md": "enable js sandbox for markdown files (default)",
         "sb_lg": "enable js sandbox for prologue/epilogue (default)",
         "md_sbf": "list of markdown-sandbox safeguards to disable",
         "lg_sbf": "list of *logue-sandbox safeguards to disable",
         "nohtml": "return html and markdown as text/html",
     },
     "others": {
-        "fk=8": 'generates per-file accesskeys,\nwhich will then be required at the "g" permission',
+        "fk=8": 'generates per-file accesskeys,\nwhich are then required at the "g" permission;\nkeys are invalidated if filesize or inode changes',
+        "fka=8": 'generates slightly weaker per-file accesskeys,\nwhich are then required at the "g" permission;\nnot affected by filesize or inode numbers',
         "davauth": "ask webdav clients to login for all folders",
         "davrt": "show lastmod time of symlink destination, not the link itself\n(note: this option is always enabled for recursive listings)",
     },
 }
 
 
 flagdescs = {k.split("=")[0]: v for tab in flagcats.values() for k, v in tab.items()}
```

### Comparing `copyparty-1.9.8/copyparty/dxml.py` & `copyparty-1.9.9/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/fsutil.py` & `copyparty-1.9.9/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/ftpd.py` & `copyparty-1.9.9/copyparty/ftpd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/httpcli.py` & `copyparty-1.9.9/copyparty/httpcli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/httpconn.py` & `copyparty-1.9.9/copyparty/httpconn.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/httpsrv.py` & `copyparty-1.9.9/copyparty/httpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/ico.py` & `copyparty-1.9.9/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/mdns.py` & `copyparty-1.9.9/copyparty/mdns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/metrics.py` & `copyparty-1.9.9/copyparty/metrics.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/mtag.py` & `copyparty-1.9.9/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/multicast.py` & `copyparty-1.9.9/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/pwhash.py` & `copyparty-1.9.9/copyparty/pwhash.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/res/COPYING.txt` & `copyparty-1.9.9/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/res/insecure.pem` & `copyparty-1.9.9/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/smbd.py` & `copyparty-1.9.9/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/ssdp.py` & `copyparty-1.9.9/copyparty/ssdp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/star.py` & `copyparty-1.9.9/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/dns.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/label.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/lex.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.9.9/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.9.9/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.9.9/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.9.9/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/qrcodegen.py` & `copyparty-1.9.9/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/stolen/surrogateescape.py` & `copyparty-1.9.9/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/sutil.py` & `copyparty-1.9.9/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/svchub.py` & `copyparty-1.9.9/copyparty/svchub.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/szip.py` & `copyparty-1.9.9/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/tcpsrv.py` & `copyparty-1.9.9/copyparty/tcpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/th_cli.py` & `copyparty-1.9.9/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/th_srv.py` & `copyparty-1.9.9/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/u2idx.py` & `copyparty-1.9.9/copyparty/u2idx.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/up2k.py` & `copyparty-1.9.9/copyparty/up2k.py`

 * *Files 0% similar despite different names*

```diff
@@ -2673,15 +2673,15 @@
 
             lsrc = src
             ldst = dst
             fs1 = bos.stat(os.path.dirname(src)).st_dev
             fs2 = bos.stat(os.path.dirname(dst)).st_dev
             if fs1 == 0 or fs2 == 0:
                 # py2 on winxp or other unsupported combination
-                raise OSError(38, "filesystem does not have st_dev")
+                raise OSError(errno.ENOSYS, "filesystem does not have st_dev")
             elif fs1 == fs2:
                 # same fs; make symlink as relative as possible
                 spl = r"[\\/]" if WINDOWS else "/"
                 nsrc = re.split(spl, src)
                 ndst = re.split(spl, dst)
                 nc = 0
                 for a, b in zip(nsrc, ndst):
@@ -3293,28 +3293,40 @@
                 raise Pebkac(400, "moving dotfiles is disabled in server config")
             elif self.args.no_dot_ren and n1 != n2:
                 raise Pebkac(400, "renaming dotfiles is disabled in server config")
 
         if bos.path.exists(dabs):
             raise Pebkac(400, "mv2: target file exists")
 
+        stl = bos.lstat(sabs)
+        try:
+            st = bos.stat(sabs)
+        except:
+            st = stl
+
         xbr = svn.flags.get("xbr")
         xar = dvn.flags.get("xar")
         if xbr:
-            st = bos.stat(sabs)
             if not runhook(
                 self.log, xbr, sabs, svp, "", uname, st.st_mtime, st.st_size, "", 0, ""
             ):
                 t = "move blocked by xbr server config: {}".format(svp)
                 self.log(t, 1)
                 raise Pebkac(405, t)
 
+        is_xvol = svn.realpath != dvn.realpath
+        if stat.S_ISLNK(stl.st_mode):
+            is_dirlink = stat.S_ISDIR(st.st_mode)
+            is_link = True
+        else:
+            is_link = is_dirlink = False
+
         bos.makedirs(os.path.dirname(dabs))
 
-        if bos.path.islink(sabs):
+        if is_dirlink:
             dlabs = absreal(sabs)
             t = "moving symlink from [{}] to [{}], target [{}]"
             self.log(t.format(sabs, dabs, dlabs))
             mt = bos.path.getmtime(sabs, False)
             bos.unlink(sabs)
             self._symlink(dlabs, dabs, dvn.flags, False, lmod=mt)
 
@@ -3329,44 +3341,30 @@
 
             return "k"
 
         c1, w, ftime_, fsize_, ip, at = self._find_from_vpath(svn.realpath, srem)
         c2 = self.cur.get(dvn.realpath)
 
         if ftime_ is None:
-            st = bos.stat(sabs)
             ftime = st.st_mtime
             fsize = st.st_size
         else:
             ftime = ftime_
             fsize = fsize_ or 0
 
-        try:
-            atomic_move(sabs, dabs)
-        except OSError as ex:
-            if ex.errno != errno.EXDEV:
-                raise
-
-            self.log("cross-device move:\n  {}\n  {}".format(sabs, dabs))
-            b1, b2 = fsenc(sabs), fsenc(dabs)
-            try:
-                shutil.copy2(b1, b2)
-            except:
-                os.unlink(b2)
-                raise
-
-            os.unlink(b1)
-
+        has_dupes = False
         if w:
             assert c1
             if c2 and c2 != c1:
                 self._copy_tags(c1, c2, w)
 
-            self._forget_file(svn.realpath, srem, c1, w, c1 != c2, fsize)
-            self._relink(w, svn.realpath, srem, dabs)
+            has_dupes = self._forget_file(svn.realpath, srem, c1, w, is_xvol, fsize)
+            if not is_xvol:
+                has_dupes = self._relink(w, svn.realpath, srem, dabs)
+
             curs.add(c1)
 
             if c2:
                 self.db_add(
                     c2,
                     {},  # skip upload hooks
                     drd,
@@ -3381,14 +3379,55 @@
                     ip or "",
                     at or 0,
                 )
                 curs.add(c2)
         else:
             self.log("not found in src db: [{}]".format(svp))
 
+        try:
+            if is_xvol and has_dupes:
+                raise OSError(errno.EXDEV, "src is symlink")
+
+            atomic_move(sabs, dabs)
+
+        except OSError as ex:
+            if ex.errno != errno.EXDEV:
+                raise
+
+            self.log("using copy+delete (%s):\n  %s\n  %s" % (ex.strerror, sabs, dabs))
+            b1, b2 = fsenc(sabs), fsenc(dabs)
+            is_link = os.path.islink(b1)  # due to _relink
+            try:
+                shutil.copy2(b1, b2)
+            except:
+                try:
+                    os.unlink(b2)
+                except:
+                    pass
+
+                if not is_link:
+                    raise
+
+                # broken symlink? keep it as-is
+                try:
+                    zb = os.readlink(b1)
+                    os.symlink(zb, b2)
+                except:
+                    os.unlink(b2)
+                    raise
+
+            if is_link:
+                try:
+                    times = (int(time.time()), int(stl.st_mtime))
+                    bos.utime(dabs, times, False)
+                except:
+                    pass
+
+            os.unlink(b1)
+
         if xar:
             runhook(self.log, xar, dabs, dvp, "", uname, 0, 0, "", 0, "")
 
         return "k"
 
     def _copy_tags(
         self, csrc , cdst , wark 
@@ -3437,19 +3476,21 @@
         cur ,
         wark ,
         drop_tags ,
         sz ,
     )  :
         """forgets file in db, fixes symlinks, does not delete"""
         srd, sfn = vsplit(vrem)
+        has_dupes = False
         self.log("forgetting {}".format(vrem))
         if wark and cur:
             self.log("found {} in db".format(wark))
             if drop_tags:
                 if self._relink(wark, ptop, vrem, ""):
+                    has_dupes = True
                     drop_tags = False
 
             if drop_tags:
                 q = "delete from mt where w=?"
                 cur.execute(q, (wark[:16],))
 
             self.db_rm(cur, srd, sfn, sz)
@@ -3469,14 +3510,16 @@
             if job:
                 t = "forgetting partial upload {} ({})"
                 p = self._vis_job_progress(job)
                 self.log(t.format(wark, p))
                 assert wark
                 del reg[wark]
 
+        return has_dupes
+
     def _relink(self, wark , sptop , srem , dabs )  :
         """
         update symlinks from file at svn/srem to dabs (rename),
         or to first remaining full if no dabs (delete)
         """
         dupes = []
         sabs = djoin(sptop, srem)
```

### Comparing `copyparty-1.9.8/copyparty/util.py` & `copyparty-1.9.9/copyparty/util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/a/partyfuse.py` & `copyparty-1.9.9/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/a/u2c.py` & `copyparty-1.9.9/copyparty/web/a/u2c.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.9.9/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/baguettebox.js.gz` & `copyparty-1.9.9/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/browser.css.gz` & `copyparty-1.9.9/copyparty/web/browser.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/browser.html` & `copyparty-1.9.9/copyparty/web/browser.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/browser.js.gz` & `copyparty-1.9.9/copyparty/web/browser.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/browser2.html` & `copyparty-1.9.9/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/cf.html` & `copyparty-1.9.9/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/dbg-audio.js.gz` & `copyparty-1.9.9/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/marked.js.gz` & `copyparty-1.9.9/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.9.9/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/mini-fa.woff` & `copyparty-1.9.9/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/prism.css.gz` & `copyparty-1.9.9/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/prism.js.gz` & `copyparty-1.9.9/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/prismd.css.gz` & `copyparty-1.9.9/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/scp.woff2` & `copyparty-1.9.9/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.9.9/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.9.9/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/md.css.gz` & `copyparty-1.9.9/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/md.html` & `copyparty-1.9.9/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/md.js.gz` & `copyparty-1.9.9/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/md2.css.gz` & `copyparty-1.9.9/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/md2.js.gz` & `copyparty-1.9.9/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/mde.css.gz` & `copyparty-1.9.9/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/mde.html` & `copyparty-1.9.9/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/mde.js.gz` & `copyparty-1.9.9/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/msg.html` & `copyparty-1.9.9/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/splash.css.gz` & `copyparty-1.9.9/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/splash.html` & `copyparty-1.9.9/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/splash.js.gz` & `copyparty-1.9.9/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/svcs.html` & `copyparty-1.9.9/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/svcs.js.gz` & `copyparty-1.9.9/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/ui.css.gz` & `copyparty-1.9.9/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/up2k.js.gz` & `copyparty-1.9.9/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/util.js.gz` & `copyparty-1.9.9/copyparty/web/util.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty/web/w.hash.js.gz` & `copyparty-1.9.9/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/copyparty.egg-info/PKG-INFO` & `copyparty-1.9.9/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.9.8
+Version: 1.9.9
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.9.8/copyparty.egg-info/SOURCES.txt` & `copyparty-1.9.9/copyparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.9.8/pyproject.toml` & `copyparty-1.9.9/pyproject.toml`

 * *Files identical despite different names*

