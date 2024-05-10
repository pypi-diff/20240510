# Comparing `tmp/cgeniepy-0.7.4.tar.gz` & `tmp/cgeniepy-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgeniepy-0.7.4.tar", last modified: Sun Nov  5 18:23:14 2023, max compression
+gzip compressed data, was "cgeniepy-0.7.5.tar", last modified: Tue Nov 14 13:08:35 2023, max compression
```

## Comparing `cgeniepy-0.7.4.tar` & `cgeniepy-0.7.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-05 18:23:14.045335 cgeniepy-0.7.4/
--rw-r--r--   0 yingrui    (501) staff       (20)     1068 2022-12-28 23:36:02.000000 cgeniepy-0.7.4/LICENSE
--rw-r--r--   0 yingrui    (501) staff       (20)     4295 2023-11-05 18:23:14.045262 cgeniepy-0.7.4/PKG-INFO
--rw-r--r--   0 yingrui    (501) staff       (20)     3853 2023-11-05 18:21:31.000000 cgeniepy-0.7.4/README.md
--rw-r--r--   0 yingrui    (501) staff       (20)      249 2023-11-05 18:21:46.000000 cgeniepy-0.7.4/pyproject.toml
--rw-r--r--   0 yingrui    (501) staff       (20)      629 2023-11-05 18:23:14.045636 cgeniepy-0.7.4/setup.cfg
-drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-05 18:23:14.032983 cgeniepy-0.7.4/src/
-drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-05 18:23:14.037388 cgeniepy-0.7.4/src/cgeniepy/
--rw-r--r--   0 yingrui    (501) staff       (20)      191 2023-10-13 13:49:10.000000 cgeniepy-0.7.4/src/cgeniepy/__init__.py
--rw-r--r--   0 yingrui    (501) staff       (20)    10106 2023-10-11 15:44:37.000000 cgeniepy-0.7.4/src/cgeniepy/_temporary.py
--rw-r--r--   0 yingrui    (501) staff       (20)     9999 2023-10-31 21:15:03.000000 cgeniepy-0.7.4/src/cgeniepy/array.py
--rw-r--r--   0 yingrui    (501) staff       (20)     7168 2023-10-12 17:39:47.000000 cgeniepy-0.7.4/src/cgeniepy/chem.py
--rw-r--r--   0 yingrui    (501) staff       (20)     2257 2023-10-12 12:40:23.000000 cgeniepy-0.7.4/src/cgeniepy/data.py
--rw-r--r--   0 yingrui    (501) staff       (20)     5650 2023-10-24 14:40:46.000000 cgeniepy-0.7.4/src/cgeniepy/ecology.py
--rw-r--r--   0 yingrui    (501) staff       (20)     5796 2023-10-12 02:13:25.000000 cgeniepy-0.7.4/src/cgeniepy/fd.py
--rw-r--r--   0 yingrui    (501) staff       (20)     7418 2023-10-12 12:53:56.000000 cgeniepy-0.7.4/src/cgeniepy/foram.py
--rw-r--r--   0 yingrui    (501) staff       (20)    10719 2023-10-24 11:34:39.000000 cgeniepy-0.7.4/src/cgeniepy/grid.py
--rw-r--r--   0 yingrui    (501) staff       (20)    10016 2023-11-04 23:47:52.000000 cgeniepy-0.7.4/src/cgeniepy/model.py
--rw-r--r--   0 yingrui    (501) staff       (20)    23122 2023-10-31 20:19:34.000000 cgeniepy-0.7.4/src/cgeniepy/plot.py
--rw-r--r--   0 yingrui    (501) staff       (20)     4486 2023-11-03 21:10:37.000000 cgeniepy-0.7.4/src/cgeniepy/skill.py
--rw-r--r--   0 yingrui    (501) staff       (20)     3344 2023-01-03 03:16:43.000000 cgeniepy-0.7.4/src/cgeniepy/utils.py
-drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-05 18:23:14.037925 cgeniepy-0.7.4/src/cgeniepy.egg-info/
--rw-r--r--   0 yingrui    (501) staff       (20)     4295 2023-11-05 18:23:14.000000 cgeniepy-0.7.4/src/cgeniepy.egg-info/PKG-INFO
--rw-r--r--   0 yingrui    (501) staff       (20)     2035 2023-11-05 18:23:14.000000 cgeniepy-0.7.4/src/cgeniepy.egg-info/SOURCES.txt
--rw-r--r--   0 yingrui    (501) staff       (20)        1 2023-11-05 18:23:14.000000 cgeniepy-0.7.4/src/cgeniepy.egg-info/dependency_links.txt
--rw-r--r--   0 yingrui    (501) staff       (20)       14 2023-11-05 18:23:14.000000 cgeniepy-0.7.4/src/cgeniepy.egg-info/top_level.txt
-drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-05 18:23:14.044841 cgeniepy-0.7.4/src/data/
--rw-r--r--   0 yingrui    (501) staff       (20)        0 2022-05-06 12:29:21.000000 cgeniepy-0.7.4/src/data/__init__.py
--rw-r--r--   0 yingrui    (501) staff       (20)      388 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/context.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiaa_Atlantic.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiaa_AtlanticALL.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiaa_Pacific.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiaa_PacificALL.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiaa_PacificEQ.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiva_Atlantic.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiva_AtlanticALL.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiva_Pacific.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiva_PacificALL.txt
--rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_GIteiiva_PacificEQ.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_ALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_Atlantic.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_AtlanticN.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_Atlantic_MOC.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_Pacific.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_PacificN.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0055c_Tanzania.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3851 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0067f_ALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3851 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_p0067f_Pacific.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_ALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_Atlantic.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_AtlanticALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_Indian.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_IndianALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_Pacific.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_PacificALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_PacificEQ.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_PacificN.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worbe2_PacificS.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_ALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_Atlantic.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_AtlanticALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_AtlanticN.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_Indian.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_IndianALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_Pacific.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_PacificALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_PacificN.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_Southern.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     5219 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worjh2_Tanzania.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worlg4_ALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worlg4_AtlanticALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worlg4_IndianALL.txt
--rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.4/src/data/mask_worlg4_PacificALL.txt
+drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-14 13:08:35.197284 cgeniepy-0.7.5/
+-rw-r--r--   0 yingrui    (501) staff       (20)     1068 2022-12-28 23:36:02.000000 cgeniepy-0.7.5/LICENSE
+-rw-r--r--   0 yingrui    (501) staff       (20)     5531 2023-11-14 13:08:35.197224 cgeniepy-0.7.5/PKG-INFO
+-rw-r--r--   0 yingrui    (501) staff       (20)     5089 2023-11-14 13:06:00.000000 cgeniepy-0.7.5/README.md
+-rw-r--r--   0 yingrui    (501) staff       (20)      250 2023-11-14 13:05:44.000000 cgeniepy-0.7.5/pyproject.toml
+-rw-r--r--   0 yingrui    (501) staff       (20)      629 2023-11-14 13:08:35.197572 cgeniepy-0.7.5/setup.cfg
+drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-14 13:08:35.183760 cgeniepy-0.7.5/src/
+drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-14 13:08:35.188388 cgeniepy-0.7.5/src/cgeniepy/
+-rw-r--r--   0 yingrui    (501) staff       (20)      191 2023-10-13 13:49:10.000000 cgeniepy-0.7.5/src/cgeniepy/__init__.py
+-rw-r--r--   0 yingrui    (501) staff       (20)    10106 2023-10-11 15:44:37.000000 cgeniepy-0.7.5/src/cgeniepy/_temporary.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     9899 2023-11-06 11:05:59.000000 cgeniepy-0.7.5/src/cgeniepy/array.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     7168 2023-10-12 17:39:47.000000 cgeniepy-0.7.5/src/cgeniepy/chem.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     1250 2023-11-13 12:15:46.000000 cgeniepy-0.7.5/src/cgeniepy/data.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     5650 2023-10-24 14:40:46.000000 cgeniepy-0.7.5/src/cgeniepy/ecology.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     5796 2023-10-12 02:13:25.000000 cgeniepy-0.7.5/src/cgeniepy/fd.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     7418 2023-10-12 12:53:56.000000 cgeniepy-0.7.5/src/cgeniepy/foram.py
+-rw-r--r--   0 yingrui    (501) staff       (20)    10719 2023-10-24 11:34:39.000000 cgeniepy-0.7.5/src/cgeniepy/grid.py
+-rw-r--r--   0 yingrui    (501) staff       (20)    10396 2023-11-13 12:20:36.000000 cgeniepy-0.7.5/src/cgeniepy/model.py
+-rw-r--r--   0 yingrui    (501) staff       (20)    23462 2023-11-08 20:22:00.000000 cgeniepy-0.7.5/src/cgeniepy/plot.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     4486 2023-11-03 21:10:37.000000 cgeniepy-0.7.5/src/cgeniepy/skill.py
+-rw-r--r--   0 yingrui    (501) staff       (20)     3344 2023-01-03 03:16:43.000000 cgeniepy-0.7.5/src/cgeniepy/utils.py
+drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-14 13:08:35.189060 cgeniepy-0.7.5/src/cgeniepy.egg-info/
+-rw-r--r--   0 yingrui    (501) staff       (20)     5531 2023-11-14 13:08:35.000000 cgeniepy-0.7.5/src/cgeniepy.egg-info/PKG-INFO
+-rw-r--r--   0 yingrui    (501) staff       (20)     2035 2023-11-14 13:08:35.000000 cgeniepy-0.7.5/src/cgeniepy.egg-info/SOURCES.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)        1 2023-11-14 13:08:35.000000 cgeniepy-0.7.5/src/cgeniepy.egg-info/dependency_links.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)       14 2023-11-14 13:08:35.000000 cgeniepy-0.7.5/src/cgeniepy.egg-info/top_level.txt
+drwxr-xr-x   0 yingrui    (501) staff       (20)        0 2023-11-14 13:08:35.196891 cgeniepy-0.7.5/src/data/
+-rw-r--r--   0 yingrui    (501) staff       (20)        0 2022-05-06 12:29:21.000000 cgeniepy-0.7.5/src/data/__init__.py
+-rw-r--r--   0 yingrui    (501) staff       (20)      388 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/context.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiaa_Atlantic.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiaa_AtlanticALL.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiaa_Pacific.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiaa_PacificALL.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiaa_PacificEQ.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiva_Atlantic.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiva_AtlanticALL.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiva_Pacific.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiva_PacificALL.txt
+-rw-r--r--   0 yingrui    (501) staff       (20)     2592 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_GIteiiva_PacificEQ.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_ALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_Atlantic.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_AtlanticN.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_Atlantic_MOC.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_Pacific.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_PacificN.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5220 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0055c_Tanzania.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3851 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0067f_ALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3851 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_p0067f_Pacific.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_ALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_Atlantic.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_AtlanticALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_Indian.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_IndianALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_Pacific.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_PacificALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_PacificEQ.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_PacificN.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worbe2_PacificS.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_ALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_Atlantic.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_AtlanticALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_AtlanticN.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_Indian.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_IndianALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_Pacific.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_PacificALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_PacificN.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_Southern.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     5219 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worjh2_Tanzania.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worlg4_ALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3923 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worlg4_AtlanticALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worlg4_IndianALL.txt
+-rwxr-xr-x   0 yingrui    (501) staff       (20)     3924 2022-10-30 15:10:51.000000 cgeniepy-0.7.5/src/data/mask_worlg4_PacificALL.txt
```

### Comparing `cgeniepy-0.7.4/LICENSE` & `cgeniepy-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/PKG-INFO` & `cgeniepy-0.7.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgeniepy
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Python package to read, analyse and visualise cGENIE Earth System Model output
 Author: Rui Ying
 Author-email: rui.ying@bristol.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 + Data visualisation
   
 ## Installation
 
 `cgeniepy` is still under active development. But welcome to try the features after downloading cgeniep from [testpypi](https://test.pypi.org/project/cgeniepy/).
 
 ```bash
-python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.4
+python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.5
 ```
 
 ## Usage
 ### 0. initialise a model instance
 ```python
 from cgeniepy.model import GenieModel
 
@@ -122,14 +122,54 @@
 	basin_data.array.values = basin_data.array.values * 1E6
 	basin_data.mean(dim='lon').plot(ax=axs[i], contour=True)
 	axs[i].title.set_text(basins[i])
 ```
 
 ![modern_po4](example_transection.png)
 
+
+### Additional Colour Palettes
+
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from cgeniepy.plot import community_palette, avail_palette
+
+def plot_colormaps(cmaps):
+    ncols = 4
+    nrows = int(np.ceil(len(cmaps) / ncols))
+    fig, axes = plt.subplots(nrows, ncols, figsize=(15, nrows))
+
+    for i, cmap_name in enumerate(cmaps):
+        row = i // ncols
+        col = i % ncols
+        ax = axes[row, col] if nrows > 1 else axes[col]
+
+        # Create a gradient image using the colormap
+        gradient = np.linspace(0, 1, 256).reshape(1, -1)
+        ax.imshow(gradient, aspect='auto', cmap=community_palette(cmap_name))
+        ax.set_title(cmap_name, fontsize=14, fontweight='bold')
+        ax.axis('off')
+
+    ## remove the unused axes
+    for i in range(len(cmaps), ncols * nrows):
+        row = i // ncols
+        col = i % ncols
+        fig.delaxes(axes[row, col])
+        
+    plt.tight_layout()
+
+# List of colormaps from cgeniepy
+cmaps_list = avail_palette()
+plot_colormaps(cmaps_list)
+```
+
+![color_map](community_palette.png)
+
+
 ## Project Roadmap 🚩
 
 - [ ] Publish the first stable version to `pypi`
 - [ ] Examples and Documentation
 - [ ] plot.py 3D facet subplots
 - [ ] plot.py more dependency of data.dimension
 - [ ] plot.py scatter data overlay
@@ -145,18 +185,22 @@
 ## Citation
 
 ```latex
 @software{cgeniepy,
   author = {Rui Ying},
   title = {A Python interface to analyse and visualise cGENIE model output},
   url = {https://github.com/ruiying-ocean/cgeniepy/},
-  version = {0.7.3},
-  date = {2023-10-23},
+  version = {0.7.5},
+  date = {2023-11-12},
 }
 ```
 
 ## Logo
 
 Logo is generated by [simple logo generator](https://github.com/creecros/simple_logo_gen) using free **righteous** font.
 
 ## Alternative
 Alex Phol's [genie_basicdiags](https://github.com/alexpohl/genie_basicdiags/)
+
+## Raise a bug
+
+Please use GitHub's Issues to raise a bug. This makes the issues traceable so that future users having the same problem can find the answer in the public domain.
```

### Comparing `cgeniepy-0.7.4/README.md` & `cgeniepy-0.7.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 + Data visualisation
   
 ## Installation
 
 `cgeniepy` is still under active development. But welcome to try the features after downloading cgeniep from [testpypi](https://test.pypi.org/project/cgeniepy/).
 
 ```bash
-python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.4
+python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.5
 ```
 
 ## Usage
 ### 0. initialise a model instance
 ```python
 from cgeniepy.model import GenieModel
 
@@ -108,14 +108,54 @@
 	basin_data.array.values = basin_data.array.values * 1E6
 	basin_data.mean(dim='lon').plot(ax=axs[i], contour=True)
 	axs[i].title.set_text(basins[i])
 ```
 
 ![modern_po4](example_transection.png)
 
+
+### Additional Colour Palettes
+
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from cgeniepy.plot import community_palette, avail_palette
+
+def plot_colormaps(cmaps):
+    ncols = 4
+    nrows = int(np.ceil(len(cmaps) / ncols))
+    fig, axes = plt.subplots(nrows, ncols, figsize=(15, nrows))
+
+    for i, cmap_name in enumerate(cmaps):
+        row = i // ncols
+        col = i % ncols
+        ax = axes[row, col] if nrows > 1 else axes[col]
+
+        # Create a gradient image using the colormap
+        gradient = np.linspace(0, 1, 256).reshape(1, -1)
+        ax.imshow(gradient, aspect='auto', cmap=community_palette(cmap_name))
+        ax.set_title(cmap_name, fontsize=14, fontweight='bold')
+        ax.axis('off')
+
+    ## remove the unused axes
+    for i in range(len(cmaps), ncols * nrows):
+        row = i // ncols
+        col = i % ncols
+        fig.delaxes(axes[row, col])
+        
+    plt.tight_layout()
+
+# List of colormaps from cgeniepy
+cmaps_list = avail_palette()
+plot_colormaps(cmaps_list)
+```
+
+![color_map](community_palette.png)
+
+
 ## Project Roadmap 🚩
 
 - [ ] Publish the first stable version to `pypi`
 - [ ] Examples and Documentation
 - [ ] plot.py 3D facet subplots
 - [ ] plot.py more dependency of data.dimension
 - [ ] plot.py scatter data overlay
@@ -131,18 +171,22 @@
 ## Citation
 
 ```latex
 @software{cgeniepy,
   author = {Rui Ying},
   title = {A Python interface to analyse and visualise cGENIE model output},
   url = {https://github.com/ruiying-ocean/cgeniepy/},
-  version = {0.7.3},
-  date = {2023-10-23},
+  version = {0.7.5},
+  date = {2023-11-12},
 }
 ```
 
 ## Logo
 
 Logo is generated by [simple logo generator](https://github.com/creecros/simple_logo_gen) using free **righteous** font.
 
 ## Alternative
 Alex Phol's [genie_basicdiags](https://github.com/alexpohl/genie_basicdiags/)
+
+## Raise a bug
+
+Please use GitHub's Issues to raise a bug. This makes the issues traceable so that future users having the same problem can find the answer in the public domain.
```

### Comparing `cgeniepy-0.7.4/setup.cfg` & `cgeniepy-0.7.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cgeniepy
-version = 0.7.4
+version = 0.7.5
 author = Rui Ying
 author_email = rui.ying@bristol.ac.uk
 description = A Python package to read, analyse and visualise cGENIE Earth System Model output
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `cgeniepy-0.7.4/src/cgeniepy/_temporary.py` & `cgeniepy-0.7.5/src/cgeniepy/_temporary.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/array.py` & `cgeniepy-0.7.5/src/cgeniepy/array.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def attr_conservation(cal_func):
     """
     A decorator to keep the attribution after array calculation
 
     This is because xarray will remove the units and long_name after calculation
     """
     def wrappered_func(self, *args, **kwargs):
-        # Temporially store the original units
-        units = self.array.units
-        long_name = self.array.long_name
-        
-        # Call the decorated function
-        result = cal_func(self, *args, **kwargs)
-        
-        # Assign back the unit to the array
-        self.array.attrs['units'] = units
-        self.array.attrs['long_name'] = long_name
-        return result
+        try:
+            # Temporially store the original units
+            units = self.array.units
+            long_name = self.array.long_name
+
+            # Call the decorated function
+            result = cal_func(self, *args, **kwargs)
+
+            # Assign back the unit to the array
+            self.array.attrs['units'] = units
+            self.array.attrs['long_name'] = long_name
+            
+            return result
+        except AttributeError:
+            print("No unit attribution detected in `self.array`, be careful of unit when doing calculation")
+            return cal_func(self, *args, **kwargs)
     return wrappered_func
 
 
 class GenieArray(GeniePlottable):
     """
     GenieArray is a class to store and compute GENIE netcdf data.
 
@@ -56,15 +61,15 @@
 
     def _set_array(self) -> xr.DataArray:
         """
         a function to be overwritten by subclass
         always return a xarray.DataArray
         """
         arr = np.nan
-        return xr.DataArray(arr)
+        return xr.DataArray(arr)    
 
     def __getitem__(self, item):
         "make GenieArray subscriptable like xarray.DataArray"
         return self.array[item]
 
     def uarray(self):
         """convert array to pint.Quantity
@@ -139,23 +144,18 @@
         Allow GenieArray to be divided by a number or another GenieArray
 
         NA/NA -> NA
         """
         quotient_array = np.zeros_like(self.array)
         
         if isinstance(other, GenieArray):
-            valid_division = np.logical_and(other.array != 0, np.isfinite(other.array))
-            valid_divisor = other.array.copy()
-            valid_divisor[~valid_division] = 1  # Set invalid divisions to 1 to avoid division by zero
-
-            quotient_array = np.divide(self.array, valid_divisor)
-            quotient_array[~valid_division] = np.nan  # Set invalid divisions to NaN
+            quotient_array = np.divide(self.array, other.array)
         else:
             # Handle division by a scalar
-            quotient_array = np.where(other != 0, self.array / other, 0)
+            quotient_array = np.divide(self.array, other)
 
         quotient = GenieArray()
         quotient.array = xr.DataArray(quotient_array)
         return quotient
 
 
     def __mul__(self, other):
```

### Comparing `cgeniepy-0.7.4/src/cgeniepy/chem.py` & `cgeniepy-0.7.5/src/cgeniepy/chem.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/ecology.py` & `cgeniepy-0.7.5/src/cgeniepy/ecology.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/fd.py` & `cgeniepy-0.7.5/src/cgeniepy/fd.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/foram.py` & `cgeniepy-0.7.5/src/cgeniepy/foram.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/grid.py` & `cgeniepy-0.7.5/src/cgeniepy/grid.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/model.py` & `cgeniepy-0.7.5/src/cgeniepy/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,18 +124,21 @@
             ## `open_dataset` to lazy load the data
             return xr.open_dataset(nc_path)
         else:            
             datasets = [xr.open_dataset(file) for file in nc_path]
             combined_ds  = xr.concat(datasets, "model")
             return combined_ds
     
-    def get_var(self, var: Union[str, List, Tuple]):
+    def get_var(self, var: Union[str, List, Tuple], unit=None):
         """
         Get the data of target variable. 
         A list of variables is supported as well.
+
+        :param var: the name of target variable
+        :param unit: the unit of target variable, usually provided in the model output
         """
         self.target_var = var
 
         ## if varstr is a string
         if isinstance(self.target_var, str):
             ## find the path to the netcdf file
             path2nc =self._lookup_ncpath(var=self.target_var)
@@ -152,15 +155,22 @@
             
             array = xr.concat(array_container, "variable")
             array.name = "ensemble_variable"
 
         ## initialise GenieArray
         target_data = GenieArray()
         target_data.array = array
-        target_data.array.attrs['units'] = format_unit(target_data.array.attrs['units'] )
+        try:
+            target_data.array.attrs['units'] = format_unit(target_data.array.attrs['units'] )
+        except KeyError:
+            print("Unit not found in cGENIE output, please check the FORTRAN code!")
+
+        ## add unit if provided
+        if not unit:
+            target_data.array.attrs['units'] = unit
                 
         return target_data
     
     def tsvar_list(self):
         """list all files biogem timeseries files
 
         If the model is an ensemble, it assumes that all models share the same
```

### Comparing `cgeniepy-0.7.4/src/cgeniepy/plot.py` & `cgeniepy-0.7.5/src/cgeniepy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """plot map based on dataframe with latitude/longitude
     using cartopy as engine
 
     :param df: pandas dataframe
     :param var: variable (column) in dataframe to plot
     :param x: coordinate attribute, default "Longitude"
     :param y: coordinate attribute, default "Latitude"
-    :param interplate: whether interpolate scatter data
+    :param interpolate: whether interpolate scatter data
 
     :returns: a map
     """
 
     if land_mask:
         ax.set_global()
         # plot land and coastline, zorder is the drawing order, smaller -> backer layer
@@ -96,36 +96,39 @@
                           zorder=1,
                           *args,
                           **kwargs)
     else:
         p = ax.scatter(
             x=df[x],
             y=df[y],
-            color_map=df[var],
+            c=df[var],
             linewidths=0.5,
             edgecolors="black",
             transform=ccrs.PlateCarree(),
             *args,
             **kwargs,
         )
 
     return p
 
-def open_cmap(cmap_name, N=256, reverse=False, alpha=None):
+def community_palette(cmap_name, N=256, reverse=False, alpha=None):
     """
-    Get a self-defined colormap
+    community-driven colormaps with multiple sources
 
-    :param cmap_name: parula, Zissou1, FantasticFox, Rushmore, Darjeeling, ODV, Section, w5m4
+    :param cmap_name: colormap name, can be found in avail_palette()
     :type cmap_name: str
 
     :returns: colormap
 
     XML data: https://sciviscolor.org/colormaps/
     txt data: from original packages
     """
+
+    if cmap_name not in avail_palette():
+        raise ValueError(f"{cmap_name} not found, accepted values are {avail_palette()}")
     
     data_dir = pathlib.Path(__file__).parent.parent
 
     file_path = None
     file_ext = None
     colors = []
     c = None
@@ -176,14 +179,19 @@
         return c.reversed()
     
     if c is None:
         raise ValueError("Colormap could not be created")
 
     return c
 
+def avail_palette():
+    """return a list of colormap names"""
+    data_dir = pathlib.Path(__file__).parent.parent
+
+    return [f.stem for f in data_dir.glob("data/colormaps/*") if f.suffix in [".txt", ".xml"]]
 
 def cbar_wrapper(plotting_func):
     """a decorator to add color bar
 
     :param plotting_func: function returning a mappable object
     :returns: plotting function with colorbar
     """
```

### Comparing `cgeniepy-0.7.4/src/cgeniepy/skill.py` & `cgeniepy-0.7.5/src/cgeniepy/skill.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy/utils.py` & `cgeniepy-0.7.5/src/cgeniepy/utils.py`

 * *Files identical despite different names*

### Comparing `cgeniepy-0.7.4/src/cgeniepy.egg-info/PKG-INFO` & `cgeniepy-0.7.5/src/cgeniepy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgeniepy
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Python package to read, analyse and visualise cGENIE Earth System Model output
 Author: Rui Ying
 Author-email: rui.ying@bristol.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 + Data visualisation
   
 ## Installation
 
 `cgeniepy` is still under active development. But welcome to try the features after downloading cgeniep from [testpypi](https://test.pypi.org/project/cgeniepy/).
 
 ```bash
-python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.4
+python3 -m pip install -i https://test.pypi.org/simple/ cgeniepy==0.7.5
 ```
 
 ## Usage
 ### 0. initialise a model instance
 ```python
 from cgeniepy.model import GenieModel
 
@@ -122,14 +122,54 @@
 	basin_data.array.values = basin_data.array.values * 1E6
 	basin_data.mean(dim='lon').plot(ax=axs[i], contour=True)
 	axs[i].title.set_text(basins[i])
 ```
 
 ![modern_po4](example_transection.png)
 
+
+### Additional Colour Palettes
+
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from cgeniepy.plot import community_palette, avail_palette
+
+def plot_colormaps(cmaps):
+    ncols = 4
+    nrows = int(np.ceil(len(cmaps) / ncols))
+    fig, axes = plt.subplots(nrows, ncols, figsize=(15, nrows))
+
+    for i, cmap_name in enumerate(cmaps):
+        row = i // ncols
+        col = i % ncols
+        ax = axes[row, col] if nrows > 1 else axes[col]
+
+        # Create a gradient image using the colormap
+        gradient = np.linspace(0, 1, 256).reshape(1, -1)
+        ax.imshow(gradient, aspect='auto', cmap=community_palette(cmap_name))
+        ax.set_title(cmap_name, fontsize=14, fontweight='bold')
+        ax.axis('off')
+
+    ## remove the unused axes
+    for i in range(len(cmaps), ncols * nrows):
+        row = i // ncols
+        col = i % ncols
+        fig.delaxes(axes[row, col])
+        
+    plt.tight_layout()
+
+# List of colormaps from cgeniepy
+cmaps_list = avail_palette()
+plot_colormaps(cmaps_list)
+```
+
+![color_map](community_palette.png)
+
+
 ## Project Roadmap 🚩
 
 - [ ] Publish the first stable version to `pypi`
 - [ ] Examples and Documentation
 - [ ] plot.py 3D facet subplots
 - [ ] plot.py more dependency of data.dimension
 - [ ] plot.py scatter data overlay
@@ -145,18 +185,22 @@
 ## Citation
 
 ```latex
 @software{cgeniepy,
   author = {Rui Ying},
   title = {A Python interface to analyse and visualise cGENIE model output},
   url = {https://github.com/ruiying-ocean/cgeniepy/},
-  version = {0.7.3},
-  date = {2023-10-23},
+  version = {0.7.5},
+  date = {2023-11-12},
 }
 ```
 
 ## Logo
 
 Logo is generated by [simple logo generator](https://github.com/creecros/simple_logo_gen) using free **righteous** font.
 
 ## Alternative
 Alex Phol's [genie_basicdiags](https://github.com/alexpohl/genie_basicdiags/)
+
+## Raise a bug
+
+Please use GitHub's Issues to raise a bug. This makes the issues traceable so that future users having the same problem can find the answer in the public domain.
```

### Comparing `cgeniepy-0.7.4/src/cgeniepy.egg-info/SOURCES.txt` & `cgeniepy-0.7.5/src/cgeniepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

