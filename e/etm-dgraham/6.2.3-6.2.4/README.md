# Comparing `tmp/etm-dgraham-6.2.3.tar.gz` & `tmp/etm-dgraham-6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.3.tar", last modified: Mon May  6 16:25:35 2024, max compression
+gzip compressed data, was "etm-dgraham-6.2.4.tar", last modified: Fri May 10 18:50:48 2024, max compression
```

## Comparing `etm-dgraham-6.2.3.tar` & `etm-dgraham-6.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.997573 etm-dgraham-6.2.3/
--rw-r--r--   0 dag        (501) staff       (20)     5909 2024-05-06 16:25:33.000000 etm-dgraham-6.2.3/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.3/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   145677 2024-05-06 16:25:35.997341 etm-dgraham-6.2.3/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144108 2024-05-06 14:19:59.000000 etm-dgraham-6.2.3/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.3/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.3/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.989570 etm-dgraham-6.2.3/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.3/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.3/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.3/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.993069 etm-dgraham-6.2.3/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.3/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.3/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-06 16:25:33.000000 etm-dgraham-6.2.3/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.3/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.3/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.3/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   330992 2024-05-06 16:25:33.000000 etm-dgraham-6.2.3/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.3/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.3/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126266 2024-05-04 14:12:33.000000 etm-dgraham-6.2.3/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.995417 etm-dgraham-6.2.3/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   145677 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-06 16:25:35.000000 etm-dgraham-6.2.3/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.3/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.3/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.3/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.3/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.2.3/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.3/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-06 16:25:35.997611 etm-dgraham-6.2.3/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.3/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.995544 etm-dgraham-6.2.3/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.3/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 16:25:35.996773 etm-dgraham-6.2.3/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.3/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.3/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.3/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.3/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.099150 etm-dgraham-6.2.4/
+-rw-r--r--   0 dag        (501) staff       (20)     5468 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-10 18:50:48.098201 etm-dgraham-6.2.4/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.4/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.4/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.091148 etm-dgraham-6.2.4/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.094185 etm-dgraham-6.2.4/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.4/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.4/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   331023 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.4/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.4/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126267 2024-05-09 23:14:48.000000 etm-dgraham-6.2.4/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.096586 etm-dgraham-6.2.4/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.4/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.4/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/namedcolors.py
+-rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.4/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-10 18:50:48.099192 etm-dgraham-6.2.4/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.4/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.096701 etm-dgraham-6.2.4/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.4/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.097673 etm-dgraham-6.2.4/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.4/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.4/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.4/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.3/CHANGES.txt` & `etm-dgraham-6.2.4/CHANGES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,39 @@
-2024-05-06 1140c15 Daniel Graham
+2024-05-10 8dcf3ad Daniel Graham
+    Tagged version 6.2.4.
+
+2024-05-10 d5e475a Daniel Graham
+    Fixed bug in processing alerts for tasks with @s and @+ entries
+    but without @r
+
+2024-05-09 3026c51 Daniel Graham
+    Minor tweaks
+
+2024-05-07 4cd650d Daniel Graham
+    README video link tweak
+
+2024-05-06 e060977 Daniel Graham
+    More video link tweaks.
+
+2024-05-06 4cd33f1 Daniel Graham
+    README tweaks
+
+2024-05-06 e12dfd3 Daniel Graham
+    Moved m4v video to YouTube (unlisted)
+
+2024-05-06 c5802f9 Daniel Graham
+    Switched to standard definition (480p) for slide show
+
+2024-05-06 e01f168 Daniel Graham
+    First pass at m4v video for README
+
+2024-05-06 80b038f Daniel Graham
+    README tweaks
+
+2024-05-06 804789b Daniel Graham
     Tagged version 6.2.3.
 
 2024-05-06 de9a6fa Daniel Graham
     Bug fix in show_goals
 
 2024-05-06 b4ad835 Daniel Graham
     Tagged version 6.2.2.
@@ -164,43 +195,7 @@
     Recognize vi vs emacs setting.
 
 2024-03-14 bfe10f2 Daniel Graham
     Tagged version 6.1.22.
 
 2024-03-14 f702181 Daniel Graham
     Tagged version 6.1.21.
-
-2024-03-14 627aa6c Daniel Graham
-    Changed type hint from | to Union for compatibility with python <
-    3.10
-
-2024-03-12 16e250c Daniel Graham
-    Tagged version 6.1.20.
-
-2024-03-12 6c56abe Daniel Graham
-    Added raise ValueError exception in format_completion when a
-    passed argument is neither a date nor a datime instance.
-
-2024-03-07 16d6676 Daniel Graham
-    Fix sort order for jobs with dates as start times.
-
-2024-03-07 867d171 Daniel Graham
-    Tagged version 6.1.19.
-
-2024-03-07 8ac164d Daniel Graham
-    Fixed bug in allowing some & arguments in task jobs. Fixed bug in
-    accounting for timezone offsets in repeating items with alarms.
-
-2024-03-06 b4bc6ef Daniel Graham
-    Tagged version 6.1.18.
-
-2024-03-06 b892344 Daniel Graham
-    Modified time and datetime formatting to show seconds when non
-    zero. Fixed maybe_alerts to avoid repetition when the
-    refresh_interval is less than a minute. Changed the default
-    refresh_interval from 60 to 6 seconds.
-
-2024-03-06 388c505 Daniel Graham
-    Enabled 'seconds' in alerts and in the duration serializer.
-
-2024-03-05 ff5ee2c Daniel Graham
-    Tagged version 6.1.17.
```

### Comparing `etm-dgraham-6.2.3/PKG-INFO` & `etm-dgraham-6.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.3
+Version: 6.2.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -130,14 +130,15 @@
 The 4 types of reminders in etm with their associated type characters:
 
 |  type   | char  |
 | ------- | ----- |
 | task    |    -  |
 | event   |    *  |
 | journal |    %  |
+| goal    |    ~  |
 | inbox   |    !  |
 
 
 See [Item Types](#item-types) for details about these item types and [Options](#options) for details about possible attributes.
 
 [↺ contents](#contents)
 
@@ -160,14 +161,18 @@
     The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
 
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
+* A goal (**~**): practice guitar 4 times per week starting this week:
+
+        ~ practice guitar @s now @q 3
+
 * Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
     This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear highlighed on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
@@ -189,29 +194,32 @@
 
 [↺ contents](#contents)
 
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
+<!-- <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/lunch_step_by_step.m4v" alt="new" title="lunch step by step" width="600px" hspace="20px"/> -->
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
-[↺ contents](#contents)
+Here is a link to a video of scheduling a lunch step by step: 
+[lunch step by step](https://www.youtube.com/watch?v=PpaRBeFFwgs).
+<!-- [↺ contents](#contents) -->
 
-#### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
+<!-- #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback} -->
 
-**FIXME** replace this section with a link to a new video
+<!-- **FIXME** replace this section with a link to a new video -->
 
 <!--
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
-        Choose a character from * (event), - (task), % (journal)
+        Choose a character from * (event), - (task), % (journal), ~ (goal)
         or ! (inbox)
 
         ────────────────────────────────────────────────────────────
         _
 
 Notice that you don't have to search for the part of the form in which you specify the type of reminder - *etm* effectively makes the one entry area the appropriate spot for this and all other input. Now enter an `*` to create an event and *etm* will prompt you for the event summary.
```

### Comparing `etm-dgraham-6.2.3/README.md` & `etm-dgraham-6.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 The 4 types of reminders in etm with their associated type characters:
 
 |  type   | char  |
 | ------- | ----- |
 | task    |    -  |
 | event   |    *  |
 | journal |    %  |
+| goal    |    ~  |
 | inbox   |    !  |
 
 
 See [Item Types](#item-types) for details about these item types and [Options](#options) for details about possible attributes.
 
 [↺ contents](#contents)
 
@@ -117,14 +118,18 @@
     The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
 
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
+* A goal (**~**): practice guitar 4 times per week starting this week:
+
+        ~ practice guitar @s now @q 3
+
 * Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
     This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear highlighed on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
@@ -146,29 +151,32 @@
 
 [↺ contents](#contents)
 
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
+<!-- <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/lunch_step_by_step.m4v" alt="new" title="lunch step by step" width="600px" hspace="20px"/> -->
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
-[↺ contents](#contents)
+Here is a link to a video of scheduling a lunch step by step: 
+[lunch step by step](https://www.youtube.com/watch?v=PpaRBeFFwgs).
+<!-- [↺ contents](#contents) -->
 
-#### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
+<!-- #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback} -->
 
-**FIXME** replace this section with a link to a new video
+<!-- **FIXME** replace this section with a link to a new video -->
 
 <!--
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
-        Choose a character from * (event), - (task), % (journal)
+        Choose a character from * (event), - (task), % (journal), ~ (goal)
         or ! (inbox)
 
         ────────────────────────────────────────────────────────────
         _
 
 Notice that you don't have to search for the part of the form in which you specify the type of reminder - *etm* effectively makes the one entry area the appropriate spot for this and all other input. Now enter an `*` to create an event and *etm* will prompt you for the event summary.
```

### Comparing `etm-dgraham-6.2.3/bump.py` & `etm-dgraham-6.2.4/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/docs/index_konnections.md` & `etm-dgraham-6.2.4/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/docs/index_usedtime.md` & `etm-dgraham-6.2.4/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/docs/multiple_timers.md` & `etm-dgraham-6.2.4/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/__main__.py` & `etm-dgraham-6.2.4/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/common.py` & `etm-dgraham-6.2.4/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/data.py` & `etm-dgraham-6.2.4/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/make_examples.py` & `etm-dgraham-6.2.4/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/model.py` & `etm-dgraham-6.2.4/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         self.interval = ()
         self.item_hsh = {}      # key -> obj
         # Note: datetime(s) require timezone and at requires itemtype
         # all else do not need item_hsh
         self.keys = {
             'itemtype': [
                 'item type',
-                'character from * (event), - (task), % (journal), ~(goal) or ! (inbox)',
+                'character from * (event), - (task), % (journal), ~ (goal) or ! (inbox)',
                 self.do_itemtype,
             ],
             'summary': [
                 'summary',
                 "brief item description. Append an '@' to add an option.",
                 self.do_summary,
             ],
@@ -7167,15 +7167,16 @@
             # this catches all alerts and beginbys for the item
             if all_tds:
                 instance_interval = [
                     today + min(all_tds),
                     tomorrow + max(all_tds),
                 ]
 
-            if 'r' in item or '+' in item:
+            # if 'r' in item or '+' in item:
+            if 'r' in item:
                 lofh = item.get('r', [])
                 rset = dr.rruleset()
 
                 for hsh in lofh:
                     freq, kwd = rrule_args(hsh)
                     kwd['dtstart'] = dtstart
                     try:
```

### Comparing `etm-dgraham-6.2.3/etm/options.py` & `etm-dgraham-6.2.4/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/report.py` & `etm-dgraham-6.2.4/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm/view.py` & `etm-dgraham-6.2.4/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -4187,15 +4187,15 @@
         mouse_support=True,
         style=style,
         full_screen=True,
         refresh_interval=1.0,
         on_invalidate=event_handler,
     )
     timer_view.stop()
-    logger.debug("XX starting {application = } XX")
+    logger.debug(f"XX starting {application = } XX")
     try:
         result = await application.run_async()
     except Exception as e:
         logger.error(f"exception {e}", exc_info=True)
     finally:
         # background_task.cancel()
         logger.info('Quitting event loop.')
```

### Comparing `etm-dgraham-6.2.3/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.3
+Version: 6.2.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -130,14 +130,15 @@
 The 4 types of reminders in etm with their associated type characters:
 
 |  type   | char  |
 | ------- | ----- |
 | task    |    -  |
 | event   |    *  |
 | journal |    %  |
+| goal    |    ~  |
 | inbox   |    !  |
 
 
 See [Item Types](#item-types) for details about these item types and [Options](#options) for details about possible attributes.
 
 [↺ contents](#contents)
 
@@ -160,14 +161,18 @@
     The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
 
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
+* A goal (**~**): practice guitar 4 times per week starting this week:
+
+        ~ practice guitar @s now @q 3
+
 * Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
     This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear highlighed on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
@@ -189,29 +194,32 @@
 
 [↺ contents](#contents)
 
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
+<!-- <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/lunch_step_by_step.m4v" alt="new" title="lunch step by step" width="600px" hspace="20px"/> -->
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
-[↺ contents](#contents)
+Here is a link to a video of scheduling a lunch step by step: 
+[lunch step by step](https://www.youtube.com/watch?v=PpaRBeFFwgs).
+<!-- [↺ contents](#contents) -->
 
-#### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
+<!-- #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback} -->
 
-**FIXME** replace this section with a link to a new video
+<!-- **FIXME** replace this section with a link to a new video -->
 
 <!--
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
-        Choose a character from * (event), - (task), % (journal)
+        Choose a character from * (event), - (task), % (journal), ~ (goal)
         or ! (inbox)
 
         ────────────────────────────────────────────────────────────
         _
 
 Notice that you don't have to search for the part of the form in which you specify the type of reminder - *etm* effectively makes the one entry area the appropriate spot for this and all other input. Now enter an `*` to create an event and *etm* will prompt you for the event summary.
```

### Comparing `etm-dgraham-6.2.3/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etmlogo.png` & `etm-dgraham-6.2.4/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etmlogo_small.png` & `etm-dgraham-6.2.4/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/etmview_agenda.png` & `etm-dgraham-6.2.4/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/namedcolors.py` & `etm-dgraham-6.2.4/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/setup.py` & `etm-dgraham-6.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/test/test_parser.py` & `etm-dgraham-6.2.4/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/utilities/colons_to_slashes.py` & `etm-dgraham-6.2.4/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/utilities/etm_in` & `etm-dgraham-6.2.4/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/utilities/inbasket` & `etm-dgraham-6.2.4/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.3/utilities/open_in_mutt` & `etm-dgraham-6.2.4/utilities/open_in_mutt`

 * *Files identical despite different names*

