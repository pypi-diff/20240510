# Comparing `tmp/kcweb-5.30.tar.gz` & `tmp/kcweb-5.301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcweb-5.30.tar", last modified: Tue Apr  9 13:41:56 2024, max compression
+gzip compressed data, was "dist\kcweb-5.301.tar", last modified: Fri May 10 09:01:12 2024, max compression
```

## Comparing `kcweb-5.30.tar` & `kcweb-5.301.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.657592 kcweb-5.30/
--rw-rw-rw-   0        0        0     1087 2024-01-15 09:20:34.000000 kcweb-5.30/LICENSE
--rw-rw-rw-   0        0        0      565 2024-04-09 13:41:56.656594 kcweb-5.30/PKG-INFO
--rw-rw-rw-   0        0        0      678 2024-01-16 14:15:14.000000 kcweb-5.30/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.550601 kcweb-5.30/kcweb/
--rw-rw-rw-   0        0        0     2379 2024-01-17 11:56:40.000000 kcweb-5.30/kcweb/Events.py
--rw-rw-rw-   0        0        0       45 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/__init__.py
--rw-rw-rw-   0        0        0    45674 2024-01-17 12:02:55.000000 kcweb-5.30/kcweb/app.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.563592 kcweb-5.30/kcweb/common/
--rw-rw-rw-   0        0        0      120 2023-12-15 12:26:49.000000 kcweb-5.30/kcweb/common/__init__.py
--rw-rw-rw-   0        0        0    63615 2024-04-08 15:22:01.000000 kcweb-5.30/kcweb/common/autoload.py
--rw-rw-rw-   0        0        0      151 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/common/globals.py
--rw-rw-rw-   0        0        0     4141 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/common/request.py
--rw-rw-rw-   0        0        0     2144 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/common/session.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.564592 kcweb-5.30/kcweb/config/
--rw-rw-rw-   0        0        0     6228 2024-04-09 13:41:53.000000 kcweb-5.30/kcweb/config/__init__.py
--rw-rw-rw-   0        0        0    11440 2024-01-16 11:22:09.000000 kcweb-5.30/kcweb/kcweb.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.566595 kcweb-5.30/kcweb/tpl/
--rw-rw-rw-   0        0        0     2124 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/tpl/err.html
--rw-rw-rw-   0        0        0      815 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/tpl/error.html
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.570592 kcweb-5.30/kcweb/utill/
--rw-rw-rw-   0        0        0     1077 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/app.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.571592 kcweb-5.30/kcweb/utill/cache/
--rw-rw-rw-   0        0        0    10456 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/cache/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.581594 kcweb-5.30/kcweb/utill/dateutil/
--rw-rw-rw-   0        0        0      230 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/__init__.py
--rw-rw-rw-   0        0        0      975 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/_common.py
--rw-rw-rw-   0        0        0      120 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/_version.py
--rw-rw-rw-   0        0        0     2773 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/easter.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.583592 kcweb-5.30/kcweb/utill/dateutil/parser/
--rw-rw-rw-   0        0        0     1787 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/parser/__init__.py
--rw-rw-rw-   0        0        0    59262 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/parser/_parser.py
--rw-rw-rw-   0        0        0    13517 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/parser/isoparser.py
--rw-rw-rw-   0        0        0    25502 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/relativedelta.py
--rw-rw-rw-   0        0        0    68282 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/rrule.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.589596 kcweb-5.30/kcweb/utill/dateutil/tz/
--rw-rw-rw-   0        0        0      568 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tz/__init__.py
--rw-rw-rw-   0        0        0    13394 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tz/_common.py
--rw-rw-rw-   0        0        0     2374 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tz/_factories.py
--rw-rw-rw-   0        0        0    64282 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tz/tz.py
--rw-rw-rw-   0        0        0    13305 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tz/win.py
--rw-rw-rw-   0        0        0       61 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/tzwin.py
--rw-rw-rw-   0        0        0     2034 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.591592 kcweb-5.30/kcweb/utill/dateutil/zoneinfo/
--rw-rw-rw-   0        0        0     6056 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/zoneinfo/__init__.py
--rw-rw-rw-   0        0        0     1772 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/dateutil/zoneinfo/rebuild.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.596593 kcweb-5.30/kcweb/utill/db/
--rw-rw-rw-   0        0        0     6576 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/model.py
--rw-rw-rw-   0        0        0    12043 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/mongodb.py
--rw-rw-rw-   0        0        0    59544 2023-10-08 13:11:36.000000 kcweb-5.30/kcweb/utill/db/mysql.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.610607 kcweb-5.30/kcweb/utill/db/pymysql/
--rw-rw-rw-   0        0        0     4873 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/__init__.py
--rw-rw-rw-   0        0        0     7985 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/_auth.py
--rw-rw-rw-   0        0        0      502 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/_compat.py
--rw-rw-rw-   0        0        0     4183 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/_socketio.py
--rw-rw-rw-   0        0        0    10542 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/charset.py
--rw-rw-rw-   0        0        0    50320 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/connections.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.618591 kcweb-5.30/kcweb/utill/db/pymysql/constants/
--rw-rw-rw-   0        0        0      884 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/CLIENT.py
--rw-rw-rw-   0        0        0      713 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/COMMAND.py
--rw-rw-rw-   0        0        0     2296 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/CR.py
--rw-rw-rw-   0        0        0    12772 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/ER.py
--rw-rw-rw-   0        0        0      405 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
--rw-rw-rw-   0        0        0      229 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/FLAG.py
--rw-rw-rw-   0        0        0      345 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
--rw-rw-rw-   0        0        0        0 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/constants/__init__.py
--rw-rw-rw-   0        0        0    12646 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/converters.py
--rw-rw-rw-   0        0        0    17774 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/cursors.py
--rw-rw-rw-   0        0        0     3825 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/err.py
--rw-rw-rw-   0        0        0      681 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/optionfile.py
--rw-rw-rw-   0        0        0    12365 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/protocol.py
--rw-rw-rw-   0        0        0      380 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/times.py
--rw-rw-rw-   0        0        0      193 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/pymysql/util.py
--rw-rw-rw-   0        0        0    23069 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/sqlite copy.py
--rw-rw-rw-   0        0        0    21956 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/db/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.623593 kcweb-5.30/kcweb/utill/filetype/
--rw-rw-rw-   0        0        0      233 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/__init__.py
--rw-rw-rw-   0        0        0     2220 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/filetype.py
--rw-rw-rw-   0        0        0     2643 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/helpers.py
--rw-rw-rw-   0        0        0     2568 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/match.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.634592 kcweb-5.30/kcweb/utill/filetype/types/
--rw-rw-rw-   0        0        0     1531 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/__init__.py
--rw-rw-rw-   0        0        0    13116 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/archive.py
--rw-rw-rw-   0        0        0     3998 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/audio.py
--rw-rw-rw-   0        0        0      706 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/base.py
--rw-rw-rw-   0        0        0     2411 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/font.py
--rw-rw-rw-   0        0        0     6616 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/image.py
--rw-rw-rw-   0        0        0      961 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/isobmff.py
--rw-rw-rw-   0        0        0     5570 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/types/video.py
--rw-rw-rw-   0        0        0     1742 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/filetype/utils.py
--rw-rw-rw-   0        0        0     3752 2023-01-10 15:00:12.000000 kcweb-5.30/kcweb/utill/http.py
--rw-rw-rw-   0        0        0    12030 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/queues.py
--rw-rw-rw-   0        0        0     8146 2023-12-11 09:13:59.000000 kcweb-5.30/kcweb/utill/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.643594 kcweb-5.30/kcweb/utill/rediss/
--rw-rw-rw-   0        0        0     1033 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/__init__.py
--rw-rw-rw-   0        0        0     4150 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/_compat.py
--rw-rw-rw-   0        0        0   150458 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/client.py
--rw-rw-rw-   0        0        0    48878 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/connection.py
--rw-rw-rw-   0        0        0     1057 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/exceptions.py
--rw-rw-rw-   0        0        0    11109 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/lock.py
--rw-rw-rw-   0        0        0    11644 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/sentinel.py
--rw-rw-rw-   0        0        0      699 2022-05-13 07:34:10.000000 kcweb-5.30/kcweb/utill/rediss/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:41:56.558592 kcweb-5.30/kcweb.egg-info/
--rw-rw-rw-   0        0        0      565 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5346 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0      339 2024-04-09 13:41:56.000000 kcweb-5.30/kcweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 13:41:56.658597 kcweb-5.30/setup.cfg
--rw-rw-rw-   0        0        0     2781 2024-04-09 13:41:46.000000 kcweb-5.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.500555 kcweb-5.301/
+-rw-rw-rw-   0        0        0     1087 2024-01-15 09:20:34.000000 kcweb-5.301/LICENSE
+-rw-rw-rw-   0        0        0      567 2024-05-10 09:01:12.500555 kcweb-5.301/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2024-01-16 14:15:14.000000 kcweb-5.301/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.400500 kcweb-5.301/kcweb/
+-rw-rw-rw-   0        0        0     2379 2024-01-17 11:56:40.000000 kcweb-5.301/kcweb/Events.py
+-rw-rw-rw-   0        0        0       45 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/__init__.py
+-rw-rw-rw-   0        0        0    45674 2024-01-17 12:02:55.000000 kcweb-5.301/kcweb/app.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.411682 kcweb-5.301/kcweb/common/
+-rw-rw-rw-   0        0        0      120 2024-04-17 07:20:10.000000 kcweb-5.301/kcweb/common/__init__.py
+-rw-rw-rw-   0        0        0    63868 2024-04-17 07:20:34.000000 kcweb-5.301/kcweb/common/autoload.py
+-rw-rw-rw-   0        0        0      151 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/common/globals.py
+-rw-rw-rw-   0        0        0     4141 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/common/request.py
+-rw-rw-rw-   0        0        0     2144 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/common/session.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.411682 kcweb-5.301/kcweb/config/
+-rw-rw-rw-   0        0        0     6229 2024-05-10 08:59:07.000000 kcweb-5.301/kcweb/config/__init__.py
+-rw-rw-rw-   0        0        0    11882 2024-04-17 07:19:03.000000 kcweb-5.301/kcweb/kcweb.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.416118 kcweb-5.301/kcweb/tpl/
+-rw-rw-rw-   0        0        0     2124 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/tpl/err.html
+-rw-rw-rw-   0        0        0      815 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/tpl/error.html
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.418715 kcweb-5.301/kcweb/utill/
+-rw-rw-rw-   0        0        0     1077 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/app.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.418715 kcweb-5.301/kcweb/utill/cache/
+-rw-rw-rw-   0        0        0    10456 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/cache/cache.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.428500 kcweb-5.301/kcweb/utill/dateutil/
+-rw-rw-rw-   0        0        0      230 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/__init__.py
+-rw-rw-rw-   0        0        0      975 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/_common.py
+-rw-rw-rw-   0        0        0      120 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/_version.py
+-rw-rw-rw-   0        0        0     2773 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/easter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.429828 kcweb-5.301/kcweb/utill/dateutil/parser/
+-rw-rw-rw-   0        0        0     1787 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/parser/__init__.py
+-rw-rw-rw-   0        0        0    59262 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/parser/_parser.py
+-rw-rw-rw-   0        0        0    13517 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/parser/isoparser.py
+-rw-rw-rw-   0        0        0    25502 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/relativedelta.py
+-rw-rw-rw-   0        0        0    68282 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/rrule.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.438057 kcweb-5.301/kcweb/utill/dateutil/tz/
+-rw-rw-rw-   0        0        0      568 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tz/__init__.py
+-rw-rw-rw-   0        0        0    13394 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tz/_common.py
+-rw-rw-rw-   0        0        0     2374 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tz/_factories.py
+-rw-rw-rw-   0        0        0    64282 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tz/tz.py
+-rw-rw-rw-   0        0        0    13305 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tz/win.py
+-rw-rw-rw-   0        0        0       61 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/tzwin.py
+-rw-rw-rw-   0        0        0     2034 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.440056 kcweb-5.301/kcweb/utill/dateutil/zoneinfo/
+-rw-rw-rw-   0        0        0     6056 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/zoneinfo/__init__.py
+-rw-rw-rw-   0        0        0     1772 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/dateutil/zoneinfo/rebuild.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.445016 kcweb-5.301/kcweb/utill/db/
+-rw-rw-rw-   0        0        0     6576 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/model.py
+-rw-rw-rw-   0        0        0    12043 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/mongodb.py
+-rw-rw-rw-   0        0        0    59544 2023-10-08 13:11:36.000000 kcweb-5.301/kcweb/utill/db/mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.460164 kcweb-5.301/kcweb/utill/db/pymysql/
+-rw-rw-rw-   0        0        0     4873 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/__init__.py
+-rw-rw-rw-   0        0        0     7985 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/_auth.py
+-rw-rw-rw-   0        0        0      502 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/_compat.py
+-rw-rw-rw-   0        0        0     4183 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/_socketio.py
+-rw-rw-rw-   0        0        0    10542 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/charset.py
+-rw-rw-rw-   0        0        0    50320 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/connections.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.469644 kcweb-5.301/kcweb/utill/db/pymysql/constants/
+-rw-rw-rw-   0        0        0      884 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/CLIENT.py
+-rw-rw-rw-   0        0        0      713 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/COMMAND.py
+-rw-rw-rw-   0        0        0     2296 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/CR.py
+-rw-rw-rw-   0        0        0    12772 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/ER.py
+-rw-rw-rw-   0        0        0      405 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
+-rw-rw-rw-   0        0        0      229 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/FLAG.py
+-rw-rw-rw-   0        0        0      345 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
+-rw-rw-rw-   0        0        0        0 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/constants/__init__.py
+-rw-rw-rw-   0        0        0    12646 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/converters.py
+-rw-rw-rw-   0        0        0    17774 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/cursors.py
+-rw-rw-rw-   0        0        0     3825 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/err.py
+-rw-rw-rw-   0        0        0      681 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/optionfile.py
+-rw-rw-rw-   0        0        0    12365 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/protocol.py
+-rw-rw-rw-   0        0        0      380 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/times.py
+-rw-rw-rw-   0        0        0      193 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/pymysql/util.py
+-rw-rw-rw-   0        0        0    23069 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/sqlite copy.py
+-rw-rw-rw-   0        0        0    21956 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/db/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.472811 kcweb-5.301/kcweb/utill/filetype/
+-rw-rw-rw-   0        0        0      233 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/__init__.py
+-rw-rw-rw-   0        0        0     2220 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/filetype.py
+-rw-rw-rw-   0        0        0     2643 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/helpers.py
+-rw-rw-rw-   0        0        0     2568 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/match.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.481897 kcweb-5.301/kcweb/utill/filetype/types/
+-rw-rw-rw-   0        0        0     1531 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/__init__.py
+-rw-rw-rw-   0        0        0    13116 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/archive.py
+-rw-rw-rw-   0        0        0     3998 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/audio.py
+-rw-rw-rw-   0        0        0      706 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/base.py
+-rw-rw-rw-   0        0        0     2411 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/font.py
+-rw-rw-rw-   0        0        0     6616 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/image.py
+-rw-rw-rw-   0        0        0      961 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/isobmff.py
+-rw-rw-rw-   0        0        0     5570 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/types/video.py
+-rw-rw-rw-   0        0        0     1742 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/filetype/utils.py
+-rw-rw-rw-   0        0        0     3845 2024-05-10 09:00:31.000000 kcweb-5.301/kcweb/utill/http.py
+-rw-rw-rw-   0        0        0    12030 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/queues.py
+-rw-rw-rw-   0        0        0     8146 2023-12-11 09:13:59.000000 kcweb-5.301/kcweb/utill/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.489546 kcweb-5.301/kcweb/utill/rediss/
+-rw-rw-rw-   0        0        0     1033 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/__init__.py
+-rw-rw-rw-   0        0        0     4150 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/_compat.py
+-rw-rw-rw-   0        0        0   150458 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/client.py
+-rw-rw-rw-   0        0        0    48878 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/connection.py
+-rw-rw-rw-   0        0        0     1057 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/exceptions.py
+-rw-rw-rw-   0        0        0    11109 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/lock.py
+-rw-rw-rw-   0        0        0    11644 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/sentinel.py
+-rw-rw-rw-   0        0        0      699 2022-05-13 07:34:10.000000 kcweb-5.301/kcweb/utill/rediss/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:01:12.405903 kcweb-5.301/kcweb.egg-info/
+-rw-rw-rw-   0        0        0      567 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5346 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      339 2024-05-10 09:01:12.000000 kcweb-5.301/kcweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:01:12.503263 kcweb-5.301/setup.cfg
+-rw-rw-rw-   0        0        0     2861 2024-05-10 08:59:39.000000 kcweb-5.301/setup.py
```

### Comparing `kcweb-5.30/LICENSE` & `kcweb-5.301/LICENSE`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/PKG-INFO` & `kcweb-5.301/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: kcweb
-Version: 5.30
+Version: 5.301
 Summary: kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售
 Home-page: UNKNOWN
 Author: 禄可集团-坤坤
 Author-email: fk1402936534@qq.com
 Maintainer: 坤坤
 Maintainer-email: fk1402936534@qq.com
 License: MIT License
 Description: 增加 kcweb 命令
-Keywords: kcweb5.30
+Keywords: kcweb5.301
 Platform: UNKNOWN
```

### Comparing `kcweb-5.30/README.md` & `kcweb-5.301/README.md`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/Events.py` & `kcweb-5.301/kcweb/Events.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/app.py` & `kcweb-5.301/kcweb/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/common/autoload.py` & `kcweb-5.301/kcweb/common/autoload.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 from mako.template import Template as kcwTemplate
 from mako.lookup import TemplateLookup
 import smtplib
 from email.mime.text import MIMEText
 from email.utils import formataddr
 from kcweb.utill import filetype
 from . import globals
-
 import asyncio,websockets,urllib,threading
+python_version=platform.python_version()
+if python_version[0:3]!='3.8':
+    print("\033[1;31;40m "+config.kcweb['name']+"-"+config.kcweb['version']+"依赖python3.8，与你现在的python"+python_version+"不兼容,推荐安装python3.8")
+    exit()
 class kcwebsocket:
     "websocket服务端"
     __clientlists=[] #所有客户端绑定的对象
     __lists=[] #所有客户端
     __group={} #组
     __uid={} #clientid绑定的uid
     async def bindUid(self,clientid,uid):
```

### Comparing `kcweb-5.30/kcweb/common/request.py` & `kcweb-5.301/kcweb/common/request.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/common/session.py` & `kcweb-5.301/kcweb/common/session.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/config/__init__.py` & `kcweb-5.301/kcweb/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 email['pwd']='' #发件人邮箱密码(如申请的smtp给的口令)
 email['sendNick']='' #发件人昵称
 email['theme']='' #默认主题
 email['recNick']='' #默认收件人昵称
 
 kcweb={}
 kcweb['name']='kcweb'                             #项目的名称
-kcweb['version']='5.30'							#项目版本
+kcweb['version']='5.301'							#项目版本
 kcweb['description']='python web框架'       #项目的简单描述
 kcweb['long_description']='kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售'     #项目详细描述
 kcweb['license']='MIT'                    #开源协议   mit开源
 kcweb['url']=''
 kcweb['author']='百里-坤坤'  					 #名字
 kcweb['author_email']='fk1402936534@qq.com' 	     #邮件地址
 kcweb['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcweb-5.30/kcweb/kcweb.py` & `kcweb-5.301/kcweb/kcweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from .common import *
 import getopt
 PATH=os.getcwd()
 sys.path.append(PATH)
 import subprocess
 def __get_cmd_par():
+    python_version=platform.python_version()
+    if python_version[0:3]!='3.8':
+        print("\033[1;31;40m "+config.kcweb['name']+"-"+config.kcweb['version']+"依赖python3.8，与你现在的python"+python_version+"不兼容")
+        exit()
     try:
         opts, args = getopt.getopt(sys.argv[1:], "h", ["project=","app=","modular=","plug=","user=","pwd=","host=","port=","timeout=","processcount=",
         "install","uninstall","pack","upload","cli"])
         # print(opts)
         # print(args)
         server=False
         if 'server' in args:
@@ -68,15 +72,22 @@
                 pack=True
             elif '--upload' == data[0]:
                 upload=True
             elif '--cli' == data[0]:
                 cli=True
             i+=1
     except Exception as e:
-        print("\033[1;31;40m有关kcweb命令的详细信息，请键入 kcweb help",e)
+        try:
+            gcs=sys.argv[1]
+        except:
+            gcs=''
+        if gcs=='-v':
+             print(config.kcweb['name']+"-"+config.kcweb['version']) 
+        else:
+            print("\033[1;31;40m有关kcweb命令的详细信息，请键入 kcweb help",e)
         return False
     else:
         return {
             'server':server,
             'project':project,'appname':appname,'modular':modular,'username':username,'password':password,'plug':plug,'host':host,'port':port,'timeout':timeout,'processcount':processcount,
             'help':help,'install':install,'uninstall':uninstall,'pack':pack,'upload':upload,'cli':cli,
             'index':i
```

### Comparing `kcweb-5.30/kcweb/tpl/err.html` & `kcweb-5.301/kcweb/tpl/err.html`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/tpl/error.html` & `kcweb-5.301/kcweb/tpl/error.html`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/app.py` & `kcweb-5.301/kcweb/utill/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/cache/cache.py` & `kcweb-5.301/kcweb/utill/cache/cache.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/_common.py` & `kcweb-5.301/kcweb/utill/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/easter.py` & `kcweb-5.301/kcweb/utill/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/parser/__init__.py` & `kcweb-5.301/kcweb/utill/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/parser/_parser.py` & `kcweb-5.301/kcweb/utill/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/parser/isoparser.py` & `kcweb-5.301/kcweb/utill/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/relativedelta.py` & `kcweb-5.301/kcweb/utill/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/rrule.py` & `kcweb-5.301/kcweb/utill/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/tz/__init__.py` & `kcweb-5.301/kcweb/utill/dateutil/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/tz/_common.py` & `kcweb-5.301/kcweb/utill/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/tz/_factories.py` & `kcweb-5.301/kcweb/utill/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/tz/tz.py` & `kcweb-5.301/kcweb/utill/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/tz/win.py` & `kcweb-5.301/kcweb/utill/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/utils.py` & `kcweb-5.301/kcweb/utill/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/zoneinfo/__init__.py` & `kcweb-5.301/kcweb/utill/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/dateutil/zoneinfo/rebuild.py` & `kcweb-5.301/kcweb/utill/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/model.py` & `kcweb-5.301/kcweb/utill/db/model.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/mongodb.py` & `kcweb-5.301/kcweb/utill/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/mysql.py` & `kcweb-5.301/kcweb/utill/db/mysql.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/__init__.py` & `kcweb-5.301/kcweb/utill/db/pymysql/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/_auth.py` & `kcweb-5.301/kcweb/utill/db/pymysql/_auth.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/_socketio.py` & `kcweb-5.301/kcweb/utill/db/pymysql/_socketio.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/charset.py` & `kcweb-5.301/kcweb/utill/db/pymysql/charset.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/connections.py` & `kcweb-5.301/kcweb/utill/db/pymysql/connections.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/constants/CLIENT.py` & `kcweb-5.301/kcweb/utill/db/pymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/constants/COMMAND.py` & `kcweb-5.301/kcweb/utill/db/pymysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/constants/CR.py` & `kcweb-5.301/kcweb/utill/db/pymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/constants/ER.py` & `kcweb-5.301/kcweb/utill/db/pymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/converters.py` & `kcweb-5.301/kcweb/utill/db/pymysql/converters.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/cursors.py` & `kcweb-5.301/kcweb/utill/db/pymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/err.py` & `kcweb-5.301/kcweb/utill/db/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/optionfile.py` & `kcweb-5.301/kcweb/utill/db/pymysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/pymysql/protocol.py` & `kcweb-5.301/kcweb/utill/db/pymysql/protocol.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/sqlite copy.py` & `kcweb-5.301/kcweb/utill/db/sqlite copy.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/db/sqlite.py` & `kcweb-5.301/kcweb/utill/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/filetype.py` & `kcweb-5.301/kcweb/utill/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/helpers.py` & `kcweb-5.301/kcweb/utill/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/match.py` & `kcweb-5.301/kcweb/utill/filetype/match.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/__init__.py` & `kcweb-5.301/kcweb/utill/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/archive.py` & `kcweb-5.301/kcweb/utill/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/audio.py` & `kcweb-5.301/kcweb/utill/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/base.py` & `kcweb-5.301/kcweb/utill/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/font.py` & `kcweb-5.301/kcweb/utill/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/image.py` & `kcweb-5.301/kcweb/utill/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/isobmff.py` & `kcweb-5.301/kcweb/utill/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/types/video.py` & `kcweb-5.301/kcweb/utill/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/filetype/utils.py` & `kcweb-5.301/kcweb/utill/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/http.py` & `kcweb-5.301/kcweb/utill/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         elif cookie:
             self.get_cookies=cookie
         if self.set_cookies:
             self.get_cookies=self.__merge(self.set_cookies,self.get_cookies)
         if self.get_cookies:
             cookies=''
             for key in self.get_cookies:
+                if not self.get_cookies[key]:
+                    self.get_cookies[key]=''
                 cookies=cookies+key+"="+self.get_cookies[key]+";"
             self.get_cookie_str=cookies
         self.get_text=response.text
         self.get_content=response.content
         self.get_response=response
         self.get_status_code=int(response.status_code)
     def __merge(self,dict1, dict2):
```

### Comparing `kcweb-5.30/kcweb/utill/queues.py` & `kcweb-5.301/kcweb/utill/queues.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/redis.py` & `kcweb-5.301/kcweb/utill/redis.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/__init__.py` & `kcweb-5.301/kcweb/utill/rediss/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/_compat.py` & `kcweb-5.301/kcweb/utill/rediss/_compat.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/client.py` & `kcweb-5.301/kcweb/utill/rediss/client.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/connection.py` & `kcweb-5.301/kcweb/utill/rediss/connection.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/exceptions.py` & `kcweb-5.301/kcweb/utill/rediss/exceptions.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/lock.py` & `kcweb-5.301/kcweb/utill/rediss/lock.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/sentinel.py` & `kcweb-5.301/kcweb/utill/rediss/sentinel.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb/utill/rediss/utils.py` & `kcweb-5.301/kcweb/utill/rediss/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/kcweb.egg-info/PKG-INFO` & `kcweb-5.301/kcweb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: kcweb
-Version: 5.30
+Version: 5.301
 Summary: kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售
 Home-page: UNKNOWN
 Author: 禄可集团-坤坤
 Author-email: fk1402936534@qq.com
 Maintainer: 坤坤
 Maintainer-email: fk1402936534@qq.com
 License: MIT License
 Description: 增加 kcweb 命令
-Keywords: kcweb5.30
+Keywords: kcweb5.301
 Platform: UNKNOWN
```

### Comparing `kcweb-5.30/kcweb.egg-info/SOURCES.txt` & `kcweb-5.301/kcweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcweb-5.30/setup.py` & `kcweb-5.301/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,174 +1,179 @@
-00000000: 0d0a 2320 7079 7468 6f6e 2073 6574 7570  ..# python setup
-00000010: 2e70 7920 7364 6973 7420 7570 6c6f 6164  .py sdist upload
-00000020: 0d0a 2320 7477 696e 6520 7570 6c6f 6164  ..# twine upload
-00000030: 202d 2d72 6570 6f73 6974 6f72 792d 7572   --repository-ur
-00000040: 6c20 6874 7470 733a 2f2f 7465 7374 2e70  l https://test.p
-00000050: 7970 692e 6f72 672f 6c65 6761 6379 2f20  ypi.org/legacy/ 
-00000060: 6469 7374 2f2a 2023 e4b8 8ae4 bca0 e588  dist/* #........
-00000070: b0e6 b58b e8af 950d 0a23 2070 6970 2069  .........# pip i
-00000080: 6e73 7461 6c6c 202d 2d69 6e64 6578 2d75  nstall --index-u
-00000090: 726c 2068 7474 7073 3a2f 2f70 7970 692e  rl https://pypi.
-000000a0: 6f72 672f 7369 6d70 6c65 2f20 6b63 7765  org/simple/ kcwe
-000000b0: 6220 2020 23e5 ae89 e8a3 85e6 b58b e8af  b   #...........
-000000c0: 95e6 9c8d e58a a1e4 b88a e79a 846b 6377  .............kcw
-000000d0: 6562 2070 6970 3320 696e 7374 616c 6c20  eb pip3 install 
-000000e0: 6b63 7765 623d 3d34 2e31 322e 3420 2d69  kcweb==4.12.4 -i
-000000f0: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
-00000100: 672f 7369 6d70 6c65 2f0d 0a23 2323 2323  g/simple/..#####
-00000110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000130: 2323 2323 2323 2323 200d 0a66 726f 6d20  ######## ..from 
-00000140: 7365 7475 7074 6f6f 6c73 2069 6d70 6f72  setuptools impor
-00000150: 7420 7365 7475 702c 2066 696e 645f 7061  t setup, find_pa
-00000160: 636b 6167 6573 2c45 7874 656e 7369 6f6e  ckages,Extension
-00000170: 0d0a 696d 706f 7274 206f 730d 0a64 6566  ..import os..def
-00000180: 2066 696c 655f 6765 745f 636f 6e74 656e   file_get_conten
-00000190: 7428 6b29 3a0d 0a20 2020 2022 e88e b7e5  t(k):..    "....
-000001a0: 8f96 e696 87e4 bbb6 e586 85e5 aeb9 220d  ..............".
-000001b0: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-000001c0: 6973 6669 6c65 286b 293a 0d0a 2020 2020  isfile(k):..    
-000001d0: 2020 2020 663d 6f70 656e 286b 2c27 7227      f=open(k,'r'
-000001e0: 2c65 6e63 6f64 696e 673d 2275 7466 2d38  ,encoding="utf-8
-000001f0: 2229 0d0a 2020 2020 2020 2020 636f 6e3d  ")..        con=
-00000200: 662e 7265 6164 2829 0d0a 2020 2020 2020  f.read()..      
-00000210: 2020 662e 636c 6f73 6528 290d 0a20 2020    f.close()..   
-00000220: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000230: 636f 6e3d 2727 0d0a 2020 2020 7265 7475  con=''..    retu
-00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
-00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
-00000260: 6527 5d3d 276b 6377 6562 2720 2020 2020  e']='kcweb'     
-00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000280: 2020 2020 2020 2020 23e9 a1b9 e79b aee7          #.......
-00000290: 9a84 e590 8de7 a7b0 200d 0a63 6f6e 666b  ........ ..confk
-000002a0: 6377 5b27 7665 7273 696f 6e27 5d3d 2735  cw['version']='5
-000002b0: 2e33 3027 0909 0909 0909 0923 e9a1 b9e7  .30'.......#....
-000002c0: 9bae e789 88e6 9cac 0d0a 636f 6e66 6b63  ..........confkc
-000002d0: 775b 2764 6573 6372 6970 7469 6f6e 275d  w['description']
-000002e0: 3d27 6b63 7765 62e4 bd9c e4b8 ba77 6562  ='kcweb......web
-000002f0: e5bc 80e5 8f91 e880 8ce8 aebe e8ae a1e7  ................
-00000300: 9a84 e9ab 98e6 80a7 e883 bde6 a186 e69e  ................
-00000310: b6ef bc8c e987 87e7 94a8 e585 a8e6 96b0  ................
-00000320: e79a 84e6 9eb6 e69e 84e6 809d e683 b3ef  ................
-00000330: bc8c e6b3 a8e9 878d e698 93e7 94a8 e680  ................
-00000340: a7e3 8082 e981 b5e5 beaa 4d49 54e5 bc80  ..........MIT...
-00000350: e6ba 90e8 aeb8 e58f afe5 8d8f e8ae aee5  ................
-00000360: 8f91 e5b8 83ef bc8c e684 8fe5 91b3 e79d  ................
-00000370: 80e4 b8aa e4ba bae5 928c e4bc 81e4 b89a  ................
-00000380: e58f afe4 bba5 e585 8de8 b4b9 e4bd bfe7  ................
-00000390: 94a8 6b63 7765 62ef bc8c e794 9ae8 87b3  ..kcweb.........
-000003a0: e585 81e8 aeb8 e68a 8ae4 bda0 e59f bae4  ................
-000003b0: ba8e 6b63 7765 62e5 bc80 e58f 91e7 9a84  ..kcweb.........
-000003c0: e5ba 94e7 94a8 e5bc 80e6 ba90 e688 96e5  ................
-000003d0: 9586 e4b8 9ae4 baa7 e593 81e5 8f91 e5b8  ................
-000003e0: 83e6 8896 e994 80e5 94ae 2720 2020 2020  ..........'     
-000003f0: 2020 23e9 a1b9 e79b aee7 9a84 e7ae 80e5    #.............
-00000400: 8d95 e68f 8fe8 bfb0 0d0a 636f 6e66 6b63  ..........confkc
-00000410: 775b 276c 6f6e 675f 6465 7363 7269 7074  w['long_descript
-00000420: 696f 6e27 5d3d 22e5 a29e e58a a020 6b63  ion']="...... kc
-00000430: 7765 6220 e591 bde4 bba4 2220 2020 2020  web ......"     
-00000440: 23e9 a1b9 e79b aee8 afa6 e7bb 86e6 8f8f  #...............
-00000450: e8bf b00d 0a63 6f6e 666b 6377 5b27 6c69  .....confkcw['li
-00000460: 6365 6e73 6527 5d3d 274d 4954 204c 6963  cense']='MIT Lic
-00000470: 656e 7365 2720 2020 2020 2020 2020 2020  ense'           
-00000480: 2020 2020 2020 2020 2023 e5bc 80e6 ba90           #......
-00000490: e58d 8fe8 aeae 2020 206d 6974 e5bc 80e6  ......   mit....
-000004a0: ba90 0d0a 636f 6e66 6b63 775b 2775 726c  ....confkcw['url
-000004b0: 275d 3d27 270d 0a63 6f6e 666b 6377 5b27  ']=''..confkcw['
-000004c0: 6175 7468 6f72 275d 3d27 e7a6 84e5 8faf  author']='......
-000004d0: e99b 86e5 9ba2 2de5 9da4 e59d a427 2020  ......-......'  
-000004e0: 0909 0909 0920 23e5 908d e5ad 970d 0a63  ..... #........c
-000004f0: 6f6e 666b 6377 5b27 6175 7468 6f72 5f65  onfkcw['author_e
-00000500: 6d61 696c 275d 3d27 666b 3134 3032 3933  mail']='fk140293
-00000510: 3635 3334 4071 712e 636f 6d27 2009 2020  6534@qq.com' .  
-00000520: 2020 2023 e982 aee4 bbb6 e59c b0e5 9d80     #............
-00000530: 0d0a 636f 6e66 6b63 775b 276d 6169 6e74  ..confkcw['maint
-00000540: 6169 6e65 7227 5d3d 27e5 9da4 e59d a427  ainer']='......'
-00000550: 2009 0909 0909 0920 23e7 bbb4 e68a a4e4   ...... #.......
-00000560: baba e591 98e7 9a84 e590 8de5 ad97 0d0a  ................
-00000570: 636f 6e66 6b63 775b 276d 6169 6e74 6169  confkcw['maintai
-00000580: 6e65 725f 656d 6169 6c27 5d3d 2766 6b31  ner_email']='fk1
-00000590: 3430 3239 3336 3533 3440 7171 2e63 6f6d  402936534@qq.com
-000005a0: 2720 2020 2023 e7bb b4e6 8aa4 e4ba bae5  '    #..........
-000005b0: 9198 e79a 84e9 82ae e4bb b6e5 9cb0 e59d  ................
-000005c0: 800d 0a64 6566 2067 6574 5f66 696c 6528  ...def get_file(
-000005d0: 666f 6c64 6572 3d27 2e2f 272c 6c69 7374  folder='./',list
-000005e0: 733d 5b5d 293a 0d0a 2020 2020 6c69 733d  s=[]):..    lis=
-000005f0: 6f73 2e6c 6973 7464 6972 2866 6f6c 6465  os.listdir(folde
-00000600: 7229 0d0a 2020 2020 666f 7220 6669 6c65  r)..    for file
-00000610: 7320 696e 206c 6973 3a0d 0a20 2020 2020  s in lis:..     
-00000620: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-00000630: 682e 6973 6669 6c65 2866 6f6c 6465 722b  h.isfile(folder+
-00000640: 222f 222b 6669 6c65 7329 3a0d 0a20 2020  "/"+files):..   
-00000650: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
-00000660: 733d 3d27 5f5f 7079 6361 6368 655f 5f27  s=='__pycache__'
-00000670: 206f 7220 6669 6c65 733d 3d27 2e67 6974   or files=='.git
-00000680: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00000690: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-000006a0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000006b0: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-000006c0: 7473 2e61 7070 656e 6428 666f 6c64 6572  ts.append(folder
-000006d0: 2b22 2f22 2b66 696c 6573 290d 0a20 2020  +"/"+files)..   
-000006e0: 2020 2020 2020 2020 2020 2020 2067 6574               get
-000006f0: 5f66 696c 6528 666f 6c64 6572 2b22 2f22  _file(folder+"/"
-00000700: 2b66 696c 6573 2c6c 6973 7473 290d 0a20  +files,lists).. 
-00000710: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00000720: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00000730: 2020 2020 7265 7475 726e 206c 6973 7473      return lists
-00000740: 0d0a 623d 6765 745f 6669 6c65 2822 6b63  ..b=get_file("kc
-00000750: 7765 6222 2c5b 276b 6377 6562 275d 290d  web",['kcweb']).
-00000760: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
-00000770: 6520 3d20 636f 6e66 6b63 775b 226e 616d  e = confkcw["nam
-00000780: 6522 5d2c 0d0a 2020 2020 7665 7273 696f  e"],..    versio
-00000790: 6e20 3d20 636f 6e66 6b63 775b 2276 6572  n = confkcw["ver
-000007a0: 7369 6f6e 225d 2c0d 0a20 2020 206b 6579  sion"],..    key
-000007b0: 776f 7264 7320 3d20 226b 6377 6562 222b  words = "kcweb"+
-000007c0: 636f 6e66 6b63 775b 2776 6572 7369 6f6e  confkcw['version
-000007d0: 275d 2c0d 0a20 2020 2064 6573 6372 6970  '],..    descrip
-000007e0: 7469 6f6e 203d 2063 6f6e 666b 6377 5b22  tion = confkcw["
-000007f0: 6465 7363 7269 7074 696f 6e22 5d2c 0d0a  description"],..
-00000800: 2020 2020 6c6f 6e67 5f64 6573 6372 6970      long_descrip
-00000810: 7469 6f6e 203d 2063 6f6e 666b 6377 5b22  tion = confkcw["
-00000820: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000830: 225d 2c0d 0a20 2020 206c 6963 656e 7365  "],..    license
-00000840: 203d 2063 6f6e 666b 6377 5b22 6c69 6365   = confkcw["lice
-00000850: 6e73 6522 5d2c 0d0a 2020 2020 6175 7468  nse"],..    auth
-00000860: 6f72 203d 2063 6f6e 666b 6377 5b22 6175  or = confkcw["au
-00000870: 7468 6f72 225d 2c0d 0a20 2020 2061 7574  thor"],..    aut
-00000880: 686f 725f 656d 6169 6c20 3d20 636f 6e66  hor_email = conf
-00000890: 6b63 775b 2261 7574 686f 725f 656d 6169  kcw["author_emai
-000008a0: 6c22 5d2c 0d0a 2020 2020 6d61 696e 7461  l"],..    mainta
-000008b0: 696e 6572 203d 2063 6f6e 666b 6377 5b22  iner = confkcw["
-000008c0: 6d61 696e 7461 696e 6572 225d 2c0d 0a20  maintainer"],.. 
-000008d0: 2020 206d 6169 6e74 6169 6e65 725f 656d     maintainer_em
-000008e0: 6169 6c20 3d20 636f 6e66 6b63 775b 226d  ail = confkcw["m
-000008f0: 6169 6e74 6169 6e65 725f 656d 6169 6c22  aintainer_email"
-00000900: 5d2c 0d0a 2020 2020 7572 6c3d 636f 6e66  ],..    url=conf
-00000910: 6b63 775b 2775 726c 275d 2c0d 0a20 2020  kcw['url'],..   
-00000920: 2070 6163 6b61 6765 7320 3d20 2062 2c0d   packages =  b,.
-00000930: 0a20 2020 2023 2064 6174 615f 6669 6c65  .    # data_file
-00000940: 733d 5b28 2753 6372 6970 7473 272c 205b  s=[('Scripts', [
-00000950: 276b 6377 6562 2f62 696e 2f6b 6377 2e65  'kcweb/bin/kcw.e
-00000960: 7865 275d 295d 2c0d 0a20 2020 2069 6e73  xe'])],..    ins
-00000970: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000980: 5b27 6775 6e69 636f 726e 3d3d 3230 2e30  ['gunicorn==20.0
-00000990: 2e34 272c 2770 796d 6f6e 676f 3e3d 332e  .4','pymongo>=3.
-000009a0: 3130 2e30 272c 274d 616b 6f3e 3d31 2e31  10.0','Mako>=1.1
-000009b0: 2e32 272c 2772 6571 7565 7374 733e 3d32  .2','requests>=2
-000009c0: 2e32 332e 3027 2c27 7369 783e 3d31 2e31  .23.0','six>=1.1
-000009d0: 322e 3027 2c27 7761 7463 6864 6f67 3e3d  2.0','watchdog>=
-000009e0: 302e 392e 3027 2c27 7765 6273 6f63 6b65  0.9.0','websocke
-000009f0: 7473 3d3d 382e 3127 5d2c 2023 e7ac ace4  ts==8.1'], #....
-00000a00: b889 e696 b9e5 8c85 0d0a 2020 2020 7061  ..........    pa
-00000a10: 636b 6167 655f 6461 7461 203d 207b 0d0a  ckage_data = {..
-00000a20: 2020 2020 2020 2020 2727 3a20 5b27 2a2e          '': ['*.
-00000a30: 6874 6d6c 272c 2027 2a2e 6a73 272c 272a  html', '*.js','*
-00000a40: 2e63 7373 272c 272a 2e6a 7067 272c 272a  .css','*.jpg','*
-00000a50: 2e70 6e67 272c 272a 2e67 6966 275d 2c0d  .png','*.gif'],.
-00000a60: 0a20 2020 207d 2c0d 0a20 2020 2065 6e74  .    },..    ent
-00000a70: 7279 5f70 6f69 6e74 7320 3d20 7b0d 0a20  ry_points = {.. 
-00000a80: 2020 2020 2020 2027 636f 6e73 6f6c 655f         'console_
-00000a90: 7363 7269 7074 7327 3a5b 0d0a 2020 2020  scripts':[..    
-00000aa0: 2020 2020 2020 2020 276b 6377 6562 203d          'kcweb =
-00000ab0: 206b 6377 6562 2e6b 6377 6562 3a65 7865   kcweb.kcweb:exe
-00000ac0: 6375 7461 626c 6527 0d0a 2020 2020 2020  cutable'..      
-00000ad0: 2020 5d0d 0a20 2020 207d 0d0a 29           ]..    }..)
+00000000: 0d0a 2320 e689 93e5 8c85 e4b8 8ae4 bca0  ..# ............
+00000010: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000020: 2073 6469 7374 2075 706c 6f61 640d 0a23   sdist upload..#
+00000030: 20e6 8993 e58c 8520 7079 7468 6f6e 2073   ...... python s
+00000040: 6574 7570 2e70 7920 7364 6973 740d 0a23  etup.py sdist..#
+00000050: 2074 7769 6e65 2075 706c 6f61 6420 2d2d   twine upload --
+00000060: 7265 706f 7369 746f 7279 2d75 726c 2068  repository-url h
+00000070: 7474 7073 3a2f 2f74 6573 742e 7079 7069  ttps://test.pypi
+00000080: 2e6f 7267 2f6c 6567 6163 792f 2064 6973  .org/legacy/ dis
+00000090: 742f 2a20 23e4 b88a e4bc a0e5 88b0 e6b5  t/* #...........
+000000a0: 8be8 af95 0d0a 2320 7069 7020 696e 7374  ......# pip inst
+000000b0: 616c 6c20 2d2d 696e 6465 782d 7572 6c20  all --index-url 
+000000c0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000000d0: 2f73 696d 706c 652f 206b 6377 6562 2020  /simple/ kcweb  
+000000e0: 2023 e5ae 89e8 a385 e6b5 8be8 af95 e69c   #..............
+000000f0: 8de5 8aa1 e4b8 8ae7 9a84 6b63 7765 6220  ..........kcweb 
+00000100: 7069 7033 2069 6e73 7461 6c6c 206b 6377  pip3 install kcw
+00000110: 6562 3d3d 342e 3132 2e34 202d 6920 6874  eb==4.12.4 -i ht
+00000120: 7470 733a 2f2f 7079 7069 2e6f 7267 2f73  tps://pypi.org/s
+00000130: 696d 706c 652f 0d0a 2320 e5ae 89e8 a385  imple/..# ......
+00000140: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000150: 2069 6e73 7461 6c6c 0d0a 2323 2323 2323   install..######
+00000160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000180: 2323 2323 2323 2320 0d0a 6672 6f6d 2073  ####### ..from s
+00000190: 6574 7570 746f 6f6c 7320 696d 706f 7274  etuptools import
+000001a0: 2073 6574 7570 2c20 6669 6e64 5f70 6163   setup, find_pac
+000001b0: 6b61 6765 732c 4578 7465 6e73 696f 6e0d  kages,Extension.
+000001c0: 0a69 6d70 6f72 7420 6f73 0d0a 6465 6620  .import os..def 
+000001d0: 6669 6c65 5f67 6574 5f63 6f6e 7465 6e74  file_get_content
+000001e0: 286b 293a 0d0a 2020 2020 22e8 8eb7 e58f  (k):..    ".....
+000001f0: 96e6 9687 e4bb b6e5 8685 e5ae b922 0d0a  ............."..
+00000200: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+00000210: 7366 696c 6528 6b29 3a0d 0a20 2020 2020  sfile(k):..     
+00000220: 2020 2066 3d6f 7065 6e28 6b2c 2772 272c     f=open(k,'r',
+00000230: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00000240: 290d 0a20 2020 2020 2020 2063 6f6e 3d66  )..        con=f
+00000250: 2e72 6561 6428 290d 0a20 2020 2020 2020  .read()..       
+00000260: 2066 2e63 6c6f 7365 2829 0d0a 2020 2020   f.close()..    
+00000270: 656c 7365 3a0d 0a20 2020 2020 2020 2063  else:..        c
+00000280: 6f6e 3d27 270d 0a20 2020 2072 6574 7572  on=''..    retur
+00000290: 6e20 636f 6e0d 0a63 6f6e 666b 6377 3d7b  n con..confkcw={
+000002a0: 7d0d 0a63 6f6e 666b 6377 5b27 6e61 6d65  }..confkcw['name
+000002b0: 275d 3d27 6b63 7765 6227 2020 2020 2020  ']='kcweb'      
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2020 2020 2020 2023 e9a1 b9e7 9bae e79a         #........
+000002e0: 84e5 908d e7a7 b020 0d0a 636f 6e66 6b63  ....... ..confkc
+000002f0: 775b 2776 6572 7369 6f6e 275d 3d27 352e  w['version']='5.
+00000300: 3330 3127 0909 0909 0909 0923 e9a1 b9e7  301'.......#....
+00000310: 9bae e789 88e6 9cac 0d0a 636f 6e66 6b63  ..........confkc
+00000320: 775b 2764 6573 6372 6970 7469 6f6e 275d  w['description']
+00000330: 3d27 6b63 7765 62e4 bd9c e4b8 ba77 6562  ='kcweb......web
+00000340: e5bc 80e5 8f91 e880 8ce8 aebe e8ae a1e7  ................
+00000350: 9a84 e9ab 98e6 80a7 e883 bde6 a186 e69e  ................
+00000360: b6ef bc8c e987 87e7 94a8 e585 a8e6 96b0  ................
+00000370: e79a 84e6 9eb6 e69e 84e6 809d e683 b3ef  ................
+00000380: bc8c e6b3 a8e9 878d e698 93e7 94a8 e680  ................
+00000390: a7e3 8082 e981 b5e5 beaa 4d49 54e5 bc80  ..........MIT...
+000003a0: e6ba 90e8 aeb8 e58f afe5 8d8f e8ae aee5  ................
+000003b0: 8f91 e5b8 83ef bc8c e684 8fe5 91b3 e79d  ................
+000003c0: 80e4 b8aa e4ba bae5 928c e4bc 81e4 b89a  ................
+000003d0: e58f afe4 bba5 e585 8de8 b4b9 e4bd bfe7  ................
+000003e0: 94a8 6b63 7765 62ef bc8c e794 9ae8 87b3  ..kcweb.........
+000003f0: e585 81e8 aeb8 e68a 8ae4 bda0 e59f bae4  ................
+00000400: ba8e 6b63 7765 62e5 bc80 e58f 91e7 9a84  ..kcweb.........
+00000410: e5ba 94e7 94a8 e5bc 80e6 ba90 e688 96e5  ................
+00000420: 9586 e4b8 9ae4 baa7 e593 81e5 8f91 e5b8  ................
+00000430: 83e6 8896 e994 80e5 94ae 2720 2020 2020  ..........'     
+00000440: 2020 23e9 a1b9 e79b aee7 9a84 e7ae 80e5    #.............
+00000450: 8d95 e68f 8fe8 bfb0 0d0a 636f 6e66 6b63  ..........confkc
+00000460: 775b 276c 6f6e 675f 6465 7363 7269 7074  w['long_descript
+00000470: 696f 6e27 5d3d 22e5 a29e e58a a020 6b63  ion']="...... kc
+00000480: 7765 6220 e591 bde4 bba4 2220 2020 2020  web ......"     
+00000490: 23e9 a1b9 e79b aee8 afa6 e7bb 86e6 8f8f  #...............
+000004a0: e8bf b00d 0a63 6f6e 666b 6377 5b27 6c69  .....confkcw['li
+000004b0: 6365 6e73 6527 5d3d 274d 4954 204c 6963  cense']='MIT Lic
+000004c0: 656e 7365 2720 2020 2020 2020 2020 2020  ense'           
+000004d0: 2020 2020 2020 2020 2023 e5bc 80e6 ba90           #......
+000004e0: e58d 8fe8 aeae 2020 206d 6974 e5bc 80e6  ......   mit....
+000004f0: ba90 0d0a 636f 6e66 6b63 775b 2775 726c  ....confkcw['url
+00000500: 275d 3d27 270d 0a63 6f6e 666b 6377 5b27  ']=''..confkcw['
+00000510: 6175 7468 6f72 275d 3d27 e7a6 84e5 8faf  author']='......
+00000520: e99b 86e5 9ba2 2de5 9da4 e59d a427 2020  ......-......'  
+00000530: 0909 0909 0920 23e5 908d e5ad 970d 0a63  ..... #........c
+00000540: 6f6e 666b 6377 5b27 6175 7468 6f72 5f65  onfkcw['author_e
+00000550: 6d61 696c 275d 3d27 666b 3134 3032 3933  mail']='fk140293
+00000560: 3635 3334 4071 712e 636f 6d27 2009 2020  6534@qq.com' .  
+00000570: 2020 2023 e982 aee4 bbb6 e59c b0e5 9d80     #............
+00000580: 0d0a 636f 6e66 6b63 775b 276d 6169 6e74  ..confkcw['maint
+00000590: 6169 6e65 7227 5d3d 27e5 9da4 e59d a427  ainer']='......'
+000005a0: 2009 0909 0909 0920 23e7 bbb4 e68a a4e4   ...... #.......
+000005b0: baba e591 98e7 9a84 e590 8de5 ad97 0d0a  ................
+000005c0: 636f 6e66 6b63 775b 276d 6169 6e74 6169  confkcw['maintai
+000005d0: 6e65 725f 656d 6169 6c27 5d3d 2766 6b31  ner_email']='fk1
+000005e0: 3430 3239 3336 3533 3440 7171 2e63 6f6d  402936534@qq.com
+000005f0: 2720 2020 2023 e7bb b4e6 8aa4 e4ba bae5  '    #..........
+00000600: 9198 e79a 84e9 82ae e4bb b6e5 9cb0 e59d  ................
+00000610: 800d 0a64 6566 2067 6574 5f66 696c 6528  ...def get_file(
+00000620: 666f 6c64 6572 3d27 2e2f 272c 6c69 7374  folder='./',list
+00000630: 733d 5b5d 293a 0d0a 2020 2020 6c69 733d  s=[]):..    lis=
+00000640: 6f73 2e6c 6973 7464 6972 2866 6f6c 6465  os.listdir(folde
+00000650: 7229 0d0a 2020 2020 666f 7220 6669 6c65  r)..    for file
+00000660: 7320 696e 206c 6973 3a0d 0a20 2020 2020  s in lis:..     
+00000670: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+00000680: 682e 6973 6669 6c65 2866 6f6c 6465 722b  h.isfile(folder+
+00000690: 222f 222b 6669 6c65 7329 3a0d 0a20 2020  "/"+files):..   
+000006a0: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
+000006b0: 733d 3d27 5f5f 7079 6361 6368 655f 5f27  s=='__pycache__'
+000006c0: 206f 7220 6669 6c65 733d 3d27 2e67 6974   or files=='.git
+000006d0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+000006e0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
+000006f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000700: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00000710: 7473 2e61 7070 656e 6428 666f 6c64 6572  ts.append(folder
+00000720: 2b22 2f22 2b66 696c 6573 290d 0a20 2020  +"/"+files)..   
+00000730: 2020 2020 2020 2020 2020 2020 2067 6574               get
+00000740: 5f66 696c 6528 666f 6c64 6572 2b22 2f22  _file(folder+"/"
+00000750: 2b66 696c 6573 2c6c 6973 7473 290d 0a20  +files,lists).. 
+00000760: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00000770: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00000780: 2020 2020 7265 7475 726e 206c 6973 7473      return lists
+00000790: 0d0a 623d 6765 745f 6669 6c65 2822 6b63  ..b=get_file("kc
+000007a0: 7765 6222 2c5b 276b 6377 6562 275d 290d  web",['kcweb']).
+000007b0: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
+000007c0: 6520 3d20 636f 6e66 6b63 775b 226e 616d  e = confkcw["nam
+000007d0: 6522 5d2c 0d0a 2020 2020 7665 7273 696f  e"],..    versio
+000007e0: 6e20 3d20 636f 6e66 6b63 775b 2276 6572  n = confkcw["ver
+000007f0: 7369 6f6e 225d 2c0d 0a20 2020 206b 6579  sion"],..    key
+00000800: 776f 7264 7320 3d20 226b 6377 6562 222b  words = "kcweb"+
+00000810: 636f 6e66 6b63 775b 2776 6572 7369 6f6e  confkcw['version
+00000820: 275d 2c0d 0a20 2020 2064 6573 6372 6970  '],..    descrip
+00000830: 7469 6f6e 203d 2063 6f6e 666b 6377 5b22  tion = confkcw["
+00000840: 6465 7363 7269 7074 696f 6e22 5d2c 0d0a  description"],..
+00000850: 2020 2020 6c6f 6e67 5f64 6573 6372 6970      long_descrip
+00000860: 7469 6f6e 203d 2063 6f6e 666b 6377 5b22  tion = confkcw["
+00000870: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000880: 225d 2c0d 0a20 2020 206c 6963 656e 7365  "],..    license
+00000890: 203d 2063 6f6e 666b 6377 5b22 6c69 6365   = confkcw["lice
+000008a0: 6e73 6522 5d2c 0d0a 2020 2020 6175 7468  nse"],..    auth
+000008b0: 6f72 203d 2063 6f6e 666b 6377 5b22 6175  or = confkcw["au
+000008c0: 7468 6f72 225d 2c0d 0a20 2020 2061 7574  thor"],..    aut
+000008d0: 686f 725f 656d 6169 6c20 3d20 636f 6e66  hor_email = conf
+000008e0: 6b63 775b 2261 7574 686f 725f 656d 6169  kcw["author_emai
+000008f0: 6c22 5d2c 0d0a 2020 2020 6d61 696e 7461  l"],..    mainta
+00000900: 696e 6572 203d 2063 6f6e 666b 6377 5b22  iner = confkcw["
+00000910: 6d61 696e 7461 696e 6572 225d 2c0d 0a20  maintainer"],.. 
+00000920: 2020 206d 6169 6e74 6169 6e65 725f 656d     maintainer_em
+00000930: 6169 6c20 3d20 636f 6e66 6b63 775b 226d  ail = confkcw["m
+00000940: 6169 6e74 6169 6e65 725f 656d 6169 6c22  aintainer_email"
+00000950: 5d2c 0d0a 2020 2020 7572 6c3d 636f 6e66  ],..    url=conf
+00000960: 6b63 775b 2775 726c 275d 2c0d 0a20 2020  kcw['url'],..   
+00000970: 2070 6163 6b61 6765 7320 3d20 2062 2c0d   packages =  b,.
+00000980: 0a20 2020 2023 2064 6174 615f 6669 6c65  .    # data_file
+00000990: 733d 5b28 2753 6372 6970 7473 272c 205b  s=[('Scripts', [
+000009a0: 276b 6377 6562 2f62 696e 2f6b 6377 2e65  'kcweb/bin/kcw.e
+000009b0: 7865 275d 295d 2c0d 0a20 2020 2069 6e73  xe'])],..    ins
+000009c0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+000009d0: 5b27 6775 6e69 636f 726e 3d3d 3230 2e30  ['gunicorn==20.0
+000009e0: 2e34 272c 2770 796d 6f6e 676f 3e3d 332e  .4','pymongo>=3.
+000009f0: 3130 2e30 272c 274d 616b 6f3e 3d31 2e31  10.0','Mako>=1.1
+00000a00: 2e32 272c 2772 6571 7565 7374 733e 3d32  .2','requests>=2
+00000a10: 2e32 332e 3027 2c27 7369 783e 3d31 2e31  .23.0','six>=1.1
+00000a20: 322e 3027 2c27 7761 7463 6864 6f67 3e3d  2.0','watchdog>=
+00000a30: 302e 392e 3027 2c27 7765 6273 6f63 6b65  0.9.0','websocke
+00000a40: 7473 3d3d 382e 3127 5d2c 2023 e7ac ace4  ts==8.1'], #....
+00000a50: b889 e696 b9e5 8c85 0d0a 2020 2020 7061  ..........    pa
+00000a60: 636b 6167 655f 6461 7461 203d 207b 0d0a  ckage_data = {..
+00000a70: 2020 2020 2020 2020 2727 3a20 5b27 2a2e          '': ['*.
+00000a80: 6874 6d6c 272c 2027 2a2e 6a73 272c 272a  html', '*.js','*
+00000a90: 2e63 7373 272c 272a 2e6a 7067 272c 272a  .css','*.jpg','*
+00000aa0: 2e70 6e67 272c 272a 2e67 6966 275d 2c0d  .png','*.gif'],.
+00000ab0: 0a20 2020 207d 2c0d 0a20 2020 2065 6e74  .    },..    ent
+00000ac0: 7279 5f70 6f69 6e74 7320 3d20 7b0d 0a20  ry_points = {.. 
+00000ad0: 2020 2020 2020 2027 636f 6e73 6f6c 655f         'console_
+00000ae0: 7363 7269 7074 7327 3a5b 0d0a 2020 2020  scripts':[..    
+00000af0: 2020 2020 2020 2020 276b 6377 6562 203d          'kcweb =
+00000b00: 206b 6377 6562 2e6b 6377 6562 3a65 7865   kcweb.kcweb:exe
+00000b10: 6375 7461 626c 6527 0d0a 2020 2020 2020  cutable'..      
+00000b20: 2020 5d0d 0a20 2020 207d 0d0a 29           ]..    }..)
```

