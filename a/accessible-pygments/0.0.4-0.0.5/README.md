# Comparing `tmp/accessible-pygments-0.0.4.tar.gz` & `tmp/accessible_pygments-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accessible-pygments-0.0.4.tar", last modified: Wed Mar 22 22:46:41 2023, max compression
+gzip compressed data, last modified: Fri May 10 11:09:37 2024, max compression
```

## Comparing `accessible-pygments-0.0.4.tar` & `accessible_pygments-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,176 @@
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.130800 accessible-pygments-0.0.4/
--rw-r--r--   0 tefa       (501) staff       (20)     1522 2022-09-26 15:10:02.000000 accessible-pygments-0.0.4/LICENSE
--rw-r--r--   0 tefa       (501) staff       (20)     5951 2023-03-22 22:46:41.130543 accessible-pygments-0.0.4/PKG-INFO
--rw-r--r--   0 tefa       (501) staff       (20)     5213 2023-02-09 23:44:51.000000 accessible-pygments-0.0.4/README.md
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.118394 accessible-pygments-0.0.4/a11y_pygments/
--rw-r--r--   0 tefa       (501) staff       (20)       72 2023-03-22 22:46:04.000000 accessible-pygments-0.0.4/a11y_pygments/__init__.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.119133 accessible-pygments-0.0.4/a11y_pygments/a11y_dark/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 18:59:23.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_dark/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4869 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_dark/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.119885 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_dark/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 18:59:54.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_dark/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4870 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_dark/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.120623 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_light/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 19:00:03.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_light/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4870 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_light/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.121294 accessible-pygments-0.0.4/a11y_pygments/a11y_light/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 19:00:12.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_light/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4870 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/a11y_light/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.121907 accessible-pygments-0.0.4/a11y_pygments/blinds_dark/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-11-07 21:23:55.000000 accessible-pygments-0.0.4/a11y_pygments/blinds_dark/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4841 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/blinds_dark/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.122519 accessible-pygments-0.0.4/a11y_pygments/blinds_light/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-11-07 21:23:55.000000 accessible-pygments-0.0.4/a11y_pygments/blinds_light/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4840 2022-11-07 21:23:55.000000 accessible-pygments-0.0.4/a11y_pygments/blinds_light/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.123049 accessible-pygments-0.0.4/a11y_pygments/github_dark/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-18 21:15:13.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4954 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.123604 accessible-pygments-0.0.4/a11y_pygments/github_dark_colorblind/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-19 16:38:45.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark_colorblind/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4949 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark_colorblind/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.124097 accessible-pygments-0.0.4/a11y_pygments/github_dark_high_contrast/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-21 17:46:33.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark_high_contrast/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4960 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_dark_high_contrast/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.124541 accessible-pygments-0.0.4/a11y_pygments/github_light/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-18 17:50:06.000000 accessible-pygments-0.0.4/a11y_pygments/github_light/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4946 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_light/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.125086 accessible-pygments-0.0.4/a11y_pygments/github_light_colorblind/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-19 17:30:50.000000 accessible-pygments-0.0.4/a11y_pygments/github_light_colorblind/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4957 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_light_colorblind/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.125574 accessible-pygments-0.0.4/a11y_pygments/github_light_high_contrast/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-21 17:46:33.000000 accessible-pygments-0.0.4/a11y_pygments/github_light_high_contrast/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4960 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/github_light_high_contrast/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.126110 accessible-pygments-0.0.4/a11y_pygments/gotthard_dark/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-11-04 20:57:22.000000 accessible-pygments-0.0.4/a11y_pygments/gotthard_dark/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4849 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/gotthard_dark/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.126652 accessible-pygments-0.0.4/a11y_pygments/gotthard_light/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-11-04 20:57:22.000000 accessible-pygments-0.0.4/a11y_pygments/gotthard_light/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4848 2023-01-24 20:49:30.000000 accessible-pygments-0.0.4/a11y_pygments/gotthard_light/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.127134 accessible-pygments-0.0.4/a11y_pygments/greative/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-11-07 22:18:52.000000 accessible-pygments-0.0.4/a11y_pygments/greative/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4847 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/greative/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.127707 accessible-pygments-0.0.4/a11y_pygments/pitaya_smoothie/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 19:00:21.000000 accessible-pygments-0.0.4/a11y_pygments/pitaya_smoothie/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     4888 2022-10-05 19:21:51.000000 accessible-pygments-0.0.4/a11y_pygments/pitaya_smoothie/style.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.128284 accessible-pygments-0.0.4/a11y_pygments/utils/
--rw-r--r--   0 tefa       (501) staff       (20)        0 2022-10-05 18:57:00.000000 accessible-pygments-0.0.4/a11y_pygments/utils/__init__.py
--rw-r--r--   0 tefa       (501) staff       (20)     1896 2023-02-09 22:39:19.000000 accessible-pygments-0.0.4/a11y_pygments/utils/utils.py
-drwxr-xr-x   0 tefa       (501) staff       (20)        0 2023-03-22 22:46:41.130180 accessible-pygments-0.0.4/accessible_pygments.egg-info/
--rw-r--r--   0 tefa       (501) staff       (20)     5951 2023-03-22 22:46:40.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/PKG-INFO
--rw-r--r--   0 tefa       (501) staff       (20)     1705 2023-03-22 22:46:41.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/SOURCES.txt
--rw-r--r--   0 tefa       (501) staff       (20)        1 2023-03-22 22:46:40.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/dependency_links.txt
--rw-r--r--   0 tefa       (501) staff       (20)     1014 2023-03-22 22:46:40.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/entry_points.txt
--rw-r--r--   0 tefa       (501) staff       (20)       14 2023-03-22 22:46:40.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/requires.txt
--rw-r--r--   0 tefa       (501) staff       (20)       14 2023-03-22 22:46:41.000000 accessible-pygments-0.0.4/accessible_pygments.egg-info/top_level.txt
--rw-r--r--   0 tefa       (501) staff       (20)       38 2023-03-22 22:46:41.130882 accessible-pygments-0.0.4/setup.cfg
--rw-r--r--   0 tefa       (501) staff       (20)     2074 2023-03-22 22:41:10.000000 accessible-pygments-0.0.4/setup.py
+-rw-r--r--   0        0        0     1269 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8180 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     5498 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     7124 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7428 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/README.md
+-rw-r--r--   0        0        0     1583 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/RELEASE.md
+-rw-r--r--   0        0        0      186 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/__init__.py
+-rw-r--r--   0        0        0     1521 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_dark/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_dark/__init__.py
+-rw-r--r--   0        0        0     4408 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_dark/style.py
+-rw-r--r--   0        0        0    88218 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_dark/images/a11y-dark.png
+-rw-r--r--   0        0        0     1262 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_dark/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_dark/__init__.py
+-rw-r--r--   0        0        0     4307 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_dark/style.py
+-rw-r--r--   0        0        0    86827 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_dark/images/a11y-high-contrast-dark.png
+-rw-r--r--   0        0        0     1491 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_light/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_light/__init__.py
+-rw-r--r--   0        0        0     4333 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_light/style.py
+-rw-r--r--   0        0        0    87358 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_light/images/a11y-high-contrast-light.png
+-rw-r--r--   0        0        0     1325 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_light/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_light/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_light/style.py
+-rw-r--r--   0        0        0    86841 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/a11y_light/images/a11y-light.png
+-rw-r--r--   0        0        0       75 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/000000.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/005b82.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/00622f.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/0072b2.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/00749c.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/008561.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/00e0e0.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/023b95.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/024c1a.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/0550ae.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/080808.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/116329.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/116633.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/141414.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/18c1c4.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/1e1e1e.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/24292f.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/3d73a9.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/437a6b.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/515151.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/5391cf.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/5ca7e4.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/622cbc.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/66707b.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/66ccee.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/66e9ec.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/6730c5.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/6e7781.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/6f98b3.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/702c00.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/72f088.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/737373.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/797979.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/7998f2.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/79c0ff.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/7ee787.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/7f4707.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8045e5.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/81b19b.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8250df.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8786ac.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8a4600.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8b949e.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/8c8c8c.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/912583.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/91cbff.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/953800.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/974eb7.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/98661b.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/996b00.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/9e86c8.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/9e8741.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/9f4e55.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/a0111f.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/a12236.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/a25e53.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/a2bffc.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/a5d6ff.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ab6369.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/abe338.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/b19db4.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/b1bac4.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/b35900.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/b89784.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/bbbbbb.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/bf5400.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/c4a2f5.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/c5e478.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/c9d1d9.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/caab6d.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/cc398b.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ccbb44.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/cf222e.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/d166a3.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/d2a8ff.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/d4d0ab.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/d71835.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/d9dee3.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/dbb7ff.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/dcc6e0.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ec8e2c.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ee6677.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f26196.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f5a394.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f5ab35.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f5f5f5.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f78c6c.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/f8f8f2.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/fad000.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/fdac54.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/fefeff.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ff7b72.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ff9492.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ffa07a.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ffa657.png
+-rw-r--r--   0        0        0       86 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ffb757.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ffd700.png
+-rw-r--r--   0        0        0       85 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/assets/ffd900.png
+-rw-r--r--   0        0        0     1305 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_dark/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_dark/__init__.py
+-rw-r--r--   0        0        0     4297 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_dark/style.py
+-rw-r--r--   0        0        0    83535 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_dark/images/blinds-dark.png
+-rw-r--r--   0        0        0     1310 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_light/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_light/__init__.py
+-rw-r--r--   0        0        0     4294 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_light/style.py
+-rw-r--r--   0        0        0    85799 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/blinds_light/images/blinds-light.png
+-rw-r--r--   0        0        0     1315 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark/__init__.py
+-rw-r--r--   0        0        0     4372 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark/style.py
+-rw-r--r--   0        0        0    90448 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark/images/github-dark.png
+-rw-r--r--   0        0        0     1351 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_colorblind/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_colorblind/__init__.py
+-rw-r--r--   0        0        0     4367 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_colorblind/style.py
+-rw-r--r--   0        0        0    89368 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_colorblind/images/github-dark-colorblind.png
+-rw-r--r--   0        0        0     1371 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_high_contrast/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_high_contrast/__init__.py
+-rw-r--r--   0        0        0     4378 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_high_contrast/style.py
+-rw-r--r--   0        0        0    89065 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_dark_high_contrast/images/github-dark-high-contrast.png
+-rw-r--r--   0        0        0     1318 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light/__init__.py
+-rw-r--r--   0        0        0     4364 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light/style.py
+-rw-r--r--   0        0        0    88025 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light/images/github-light.png
+-rw-r--r--   0        0        0     1258 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_colorblind/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_colorblind/__init__.py
+-rw-r--r--   0        0        0     4375 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_colorblind/style.py
+-rw-r--r--   0        0        0    88078 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_colorblind/images/github-light-colorblind.png
+-rw-r--r--   0        0        0     1374 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_high_contrast/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_high_contrast/__init__.py
+-rw-r--r--   0        0        0     4378 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_high_contrast/style.py
+-rw-r--r--   0        0        0    88613 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/github_light_high_contrast/images/github-light-high-contrast.png
+-rw-r--r--   0        0        0     1315 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_dark/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_dark/__init__.py
+-rw-r--r--   0        0        0     4288 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_dark/style.py
+-rw-r--r--   0        0        0    88150 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_dark/images/gotthard-dark.png
+-rw-r--r--   0        0        0     1311 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_light/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_light/__init__.py
+-rw-r--r--   0        0        0     4287 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_light/style.py
+-rw-r--r--   0        0        0    86369 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/gotthard_light/images/gotthard-light.png
+-rw-r--r--   0        0        0     1290 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/greative/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/greative/__init__.py
+-rw-r--r--   0        0        0     4288 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/greative/style.py
+-rw-r--r--   0        0        0    86732 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/greative/images/greative.png
+-rw-r--r--   0        0        0     1542 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/pitaya_smoothie/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/pitaya_smoothie/__init__.py
+-rw-r--r--   0        0        0     4300 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/pitaya_smoothie/style.py
+-rw-r--r--   0        0        0    86264 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/pitaya_smoothie/images/pitaya-smoothie.png
+-rw-r--r--   0        0        0        0 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/utils/__init__.py
+-rw-r--r--   0        0        0     2030 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/utils/utils.py
+-rw-r--r--   0        0        0     4307 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/a11y_pygments/utils/wcag_contrast.py
+-rw-r--r--   0        0        0     1836 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1522 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4066 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10286 2024-05-10 11:09:37.000000 accessible_pygments-0.0.5/PKG-INFO
```

### Comparing `accessible-pygments-0.0.4/LICENSE` & `accessible_pygments-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `accessible-pygments-0.0.4/a11y_pygments/a11y_dark/style.py` & `accessible_pygments-0.0.5/a11y_pygments/blinds_dark/style.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#d4d0ab"
-    red = "#ffa07a"
-    orange = "#f5ab35"
-    yellow = "#ffd700"
-    green = "#abe338"
-    blue = "#00e0e0"
-    purple = "#dcc6e0"
-    black = "#f8f8f2"
+    comment = "#8C8C8C"
+    orange = "#ee6677"
+    yellow = "#ccbb44"
+    green = "#66ccee"
+    blue = "#5391CF"
+    purple = "#D166A3"
+    black = "#bbbbbb"
 
 
 class Theme(Style):
     """
-    This style mimics the a11 light theme from eric bailey's accessible themes.
+    This style mimics the blinds dark theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#2b2b2b"
-    highlight_color = "#ffd9002e"
+    background_color = "#242424"
+    highlight_color = "#66666691"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.purple,   # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.blue,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k' #####
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.orange,   # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.yellow,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.green,  # class: 'kt'
+        Operator: Colors.orange,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.blue,  # class: 'n'
+        Name.Attribute: Colors.purple,  # class: 'na'
+        Name.Builtin: Colors.green,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.green,  # class: 'bp'
+        Name.Class: Colors.orange,  # class: 'nc'
+        Name.Constant: Colors.orange,  # class: 'no'
+        Name.Decorator: Colors.yellow,  # class: 'nd'
+        Name.Entity: Colors.yellow,  # class: 'ni'
+        Name.Exception: Colors.blue,  # class: 'ne'
+        Name.Function: Colors.green,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.green,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.blue,     # class: 'nt'
-        Name.Variable:             Colors.red,      # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.green,  # class: 'nt'
+        Name.Variable: Colors.blue,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.black,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.blue,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.green,    # class: 'sb'
+        String: Colors.purple,  # class: 's'
+        # String.Backtick:           Colors.green,   # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.red,      # class: 'sr'
+        String.Regex: Colors.purple,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.orange,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_dark/style.py` & `accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_light/style.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#ffd900"
-    red = "#ffa07a"
-    orange = "#ffd900"
-    yellow = "#ffd900"
-    green = "#abe338"
-    blue = "#00e0e0"
-    purple = "#dcc6e0"
-    black = "#f8f8f2"
+    comment = "#515151"
+    red = "#a12236"
+    orange = "#7f4707"
+    magenta = "#912583"
+    green = "#00622f"
+    blue = "#005b82"
+    purple = "#6730c5"
+    black = "#080808"
 
 
 class Theme(Style):
     """
-    This style mimics the a11 light theme from eric bailey's accessible themes.
+    This style mimics the a11y-light theme (but with more contrast) from eric bailey's accessible themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#2b2b2b"
-    highlight_color = "#ffd9002e"
+    background_color = "#fefefe"
+    highlight_color = "#fae4c2"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.purple,   # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.orange,   # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.yellow,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.orange,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.magenta,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.blue,     # class: 'nt'
-        Name.Variable:             Colors.red,      # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.blue,  # class: 'nt'
+        Name.Variable: Colors.red,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.green,    # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.green,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.red,      # class: 'sr'
+        String.Regex: Colors.red,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
     }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/a11y_high_contrast_light/style.py` & `accessible_pygments-0.0.5/a11y_pygments/gotthard_dark/style.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#797129"
-    red = "#d91e18"
-    orange = "#797129"
-    yellow = "#797129"
-    green = "#008000"
-    blue = "#007faa"
-    purple = "#7928a1"
-    black = "#545454"
+    comment = "#F5F5F5"
+    red = "#AB6369"
+    orange = "#B89784"
+    yellow = "#CAAB6D"
+    green = "#81B19B"
+    blue = "#6F98B3"
+    purple = "#b19db4"
+    black = "#F5F5F5"
 
 
 class Theme(Style):
     """
-    This style mimics the a11 light theme from eric bailey's accessible themes.
+    This style mimics the gotthard dark theme from vscode.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#fefefe"
-    highlight_color = "#7971292e"
+    background_color = "#000000"
+    highlight_color = "#4c4b4be8"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.purple,   # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.purple,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.red,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.orange,   # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.yellow,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.green,  # class: 'kt'
+        Operator: Colors.blue,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.purple,  # class: 'na'
+        Name.Builtin: Colors.green,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.green,  # class: 'bp'
+        Name.Class: Colors.yellow,  # class: 'nc'
+        Name.Constant: Colors.red,  # class: 'no'
+        Name.Decorator: Colors.green,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.red,  # class: 'ne'
+        Name.Function: Colors.purple,  # class: 'nf'
+        Name.Property: Colors.purple,  # class: 'py'
+        Name.Label: Colors.green,  # class: 'nl'
+        Name.Namespace: Colors.yellow,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.blue,     # class: 'nt'
-        Name.Variable:             Colors.red,      # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.red,  # class: 'nt'
+        Name.Variable: Colors.comment,  # class: 'nv'
+        Name.Variable.Magic: Colors.comment,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.red,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.purple,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.green,    # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.yellow,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
-        # String.Escape:             "",            # class: 'se'
+        String.Escape: Colors.blue,  # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.red,      # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.green,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
+        Generic.Deleted: Colors.red,  # class: 'gd',
+        # Generic.Emph:              "italic",      # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Heading: Colors.green,  # class: 'gh'
+        Generic.Subheading: Colors.green,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
     }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/a11y_light/style.py` & `accessible_pygments-0.0.5/a11y_pygments/blinds_light/style.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#696969"
-    red = "#d91e18"
-    orange = "#aa5d00"
-    yellow = "#aa5d00"
-    green = "#008000"
-    blue = "#007faa"
-    purple = "#7928a1"
-    black = "#545454"
+    comment = "#737373"
+    orange = "#BF5400"
+    yellow = "#996B00"
+    green = "#008561"
+    blue = "#0072b2"
+    purple = "#CC398B"
+    black = "#000000"
 
 
 class Theme(Style):
     """
-    This style mimics the a11 light theme from eric bailey's accessible themes.
+    This style mimics the blinds light theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#fefefe"
-    highlight_color = "#7971292e"
+    background_color = "#fcfcfc"
+    highlight_color = "#add6ff"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.purple,   # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.blue,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k' #####
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.orange,   # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.yellow,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.green,  # class: 'kt'
+        Operator: Colors.orange,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.blue,  # class: 'n'
+        Name.Attribute: Colors.purple,  # class: 'na'
+        Name.Builtin: Colors.green,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.green,  # class: 'bp'
+        Name.Class: Colors.orange,  # class: 'nc'
+        Name.Constant: Colors.orange,  # class: 'no'
+        Name.Decorator: Colors.yellow,  # class: 'nd'
+        Name.Entity: Colors.blue,  # class: 'ni'
+        Name.Exception: Colors.blue,  # class: 'ne'
+        Name.Function: Colors.green,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.green,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.blue,     # class: 'nt'
-        Name.Variable:             Colors.red,      # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.green,  # class: 'nt'
+        Name.Variable: Colors.blue,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.black,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.blue,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.green,    # class: 'sb'
+        String: Colors.purple,  # class: 's'
+        # String.Backtick:           Colors.green,   # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.red,      # class: 'sr'
+        String.Regex: Colors.purple,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.orange,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
     }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/blinds_light/style.py` & `accessible_pygments-0.0.5/a11y_pygments/a11y_high_contrast_dark/style.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#737373"
-    orange = "#BF5400"
-    yellow = "#996B00"
-    green = "#008561"
-    blue = "#0072b2"
-    purple = "#CC398B"
-    black = "#000000"
+    comment = "#ffd900"
+    red = "#ffa07a"
+    orange = "#ffd900"
+    yellow = "#ffd900"
+    green = "#abe338"
+    blue = "#00e0e0"
+    purple = "#dcc6e0"
+    black = "#f8f8f2"
 
 
 class Theme(Style):
     """
-    This style mimics the blinds light theme from vscode themes.
+    This style mimics the a11 light theme from eric bailey's accessible themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#fcfcfc"
-    highlight_color = "#add6ff"
+    background_color = "#2b2b2b"
+    highlight_color = "#ffd9002e"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.blue,     # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k' #####
-        Keyword.Constant:          Colors.purple,   # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.green,    # class: 'kt'
-
-        Operator:                  Colors.orange,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.blue,     # class: 'n'
-        Name.Attribute:            Colors.purple,   # class: 'na'
-        Name.Builtin:              Colors.green,    # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.green,    # class: 'bp'
-        Name.Class:                Colors.orange,   # class: 'nc'
-        Name.Constant:             Colors.orange,   # class: 'no'
-        Name.Decorator:            Colors.yellow,   # class: 'nd'
-        Name.Entity:               Colors.blue,     # class: 'ni'
-        Name.Exception:            Colors.blue,     # class: 'ne'
-        Name.Function:             Colors.green,    # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.green,    # class: 'nn'
+        Keyword.Type: Colors.orange,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.yellow,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.blue,     # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.blue,  # class: 'nt'
+        Name.Variable: Colors.red,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.black,    # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.blue,     # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.purple,   # class: 's'
-        #String.Backtick:           Colors.green,   # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.green,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.purple,   # class: 'sr'
+        String.Regex: Colors.red,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.orange,   # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
     }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_dark/style.py` & `accessible_pygments-0.0.5/a11y_pygments/a11y_light/style.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#8b949e"  # grey[2]
-    red = "#ff7b72"  # red[3]
-    orange = "#ffa657"  # orange[2]
-    green = "#7ee787"  # green[1]
-    blue = "#79c0ff"  # blue[2]
-    purple = "#d2a8ff"  # purple[2]
-    black = "#C9D1D9"  # fg.default
+    comment = "#515151"
+    red = "#d71835"
+    orange = "#7f4707"
+    yellow = "#7f4707"
+    green = "#116633"
+    blue = "#00749c"
+    purple = "#8045e5"
+    black = "#1e1e1e"
 
 
 class Theme(Style):
     """
-    This style mimics the github dark default theme from vs code themes.
+    This style inspired by the a11y-light theme from eric bailey's accessible themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#0d1117"  # canvas.default
-    highlight_color = "#6e768182"  # accent.fg
+    background_color = "#f2f2f2"
+    highlight_color = "#fdf2e2"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.orange,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.yellow,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.blue,  # class: 'nt'
+        Name.Variable: Colors.red,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.green,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.red,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        # Generic.Error:             "",            # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_dark_colorblind/style.py` & `accessible_pygments-0.0.5/a11y_pygments/github_light_colorblind/style.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,104 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#b1bac4"  # grey[2]
-    red = "#ec8e2c"  # red[3]
-    orange = "#fdac54"  # orange[2]
-    green = "#a5d6ff"  # green[1]
-    blue = "#79c0ff"  # blue[2]
-    purple = "#d2a8ff"  # purple[2]
-    black = "#C9D1D9"  # fg.default
+    comment = "#6e7781"  # grey[5]
+    red = "#b35900"  # red[5]
+    orange = "#8a4600"  # orange[6]
+    green = "#0550ae"  # green[6]
+    blue = "#0550ae"  # blue[6]
+    purple = "#8250df"  # purple[5]
+    black = "#24292f"  # fg.default
 
 
 class Theme(Style):
     """
-    This style mimics the github dark colorblind theme from vscode.
+    This style mimics the github light colorblind theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#0d1117"  # canvas.default
-    highlight_color = "#58a6ff70"  # accent.fg
+    background_color = "#ffffff"  # canvas.default
+    highlight_color = "#0969da4a"  # accent.fg
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.red,  # class: 'k'
+        Keyword.Constant: Colors.blue,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.red,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.purple,  # class: 'n'
+        Name.Attribute: Colors.orange,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.green,  # class: 'nt'
+        Name.Variable: Colors.orange,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.blue,  # class: 's'
+        String.Backtick: Colors.blue,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        Generic.Error: Colors.red,  # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_dark_high_contrast/style.py` & `accessible_pygments-0.0.5/a11y_pygments/greative/style.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#d9dee3"  # grey[2]
-    red = "#ff9492"  # red[3]
-    orange = "#ffb757"  # orange[2]
-    green = "#72f088"  # green[1]
-    blue = "#91cbff"  # blue[2]
-    purple = "#dbb7ff"  # purple[2]
-    black = "#C9D1D9"  # fg.default
+    comment = "#797979"
+    orange = "#F78C6C"
+    yellow = "#9e8741"
+    green = "#c5e478"
+    blue = "#a2bffc"
+    cyan = "#5ca7e4"
+    purple = "#9e86c8"
+    black = "#a2bffc"
 
 
 class Theme(Style):
     """
-    This style mimics the github dark high contrast theme from vs code themes.
+    This style mimics greative theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#0d1117"  # canvas.default
-    highlight_color = "#58a6ff70"  # accent.fg
+    background_color = "#010726"
+    highlight_color = "#473d18"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.blue,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.green,  # class: 'kt'
+        Operator: Colors.orange,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.blue,  # class: 'n'
+        Name.Attribute: Colors.purple,  # class: 'na'
+        Name.Builtin: Colors.green,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.green,  # class: 'bp'
+        Name.Class: Colors.orange,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.yellow,  # class: 'nd'
+        Name.Entity: Colors.yellow,  # class: 'ni'
+        Name.Exception: Colors.blue,  # class: 'ne'
+        Name.Function: Colors.purple,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.green,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.cyan,  # class: 'nt'
+        Name.Variable: Colors.green,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.purple,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.blue,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.yellow,  # class: 's'
+        # String.Backtick:           Colors.green,   # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
-        # String.Escape:             "",            # class: 'se'
+        String.Escape: Colors.orange,  # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.cyan,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.orange,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        # Generic.Error:             "",            # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_light/style.py` & `accessible_pygments-0.0.5/a11y_pygments/github_light_high_contrast/style.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,104 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#6e7781"  # grey[5]
-    red = "#cf222e"  # red[5]
-    orange = "#953800"  # orange[6]
-    green = "#116329"  # green[6]
-    blue = "#0550ae"  # blue[6]
-    purple = "#8250df"  # purple[5]
+    comment = "#66707b"  # grey[5]
+    red = "#a0111f"  # red[5]
+    orange = "#702c00"  # orange[6]
+    green = "#024c1a"  # green[6]
+    blue = "#023b95"  # blue[6]
+    purple = "#622cbc"  # purple[5]
     black = "#24292f"  # fg.default
 
 
 class Theme(Style):
     """
-    This style mimics the github light theme from vscode themes.
+    This style mimics the github light high contrast theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
     background_color = "#ffffff"  # canvas.default
     highlight_color = "#0969da4a"  # accent.fg
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.red,  # class: 'k'
+        Keyword.Constant: Colors.blue,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.red,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.purple,  # class: 'n'
+        Name.Attribute: Colors.orange,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.green,  # class: 'nt'
+        Name.Variable: Colors.orange,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.blue,  # class: 's'
+        String.Backtick: Colors.blue,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        Generic.Error: Colors.red,  # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_light_colorblind/style.py` & `accessible_pygments-0.0.5/a11y_pygments/github_light/style.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,102 +1,104 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
     comment = "#6e7781"  # grey[5]
-    red = "#b35900"  # red[5]
-    orange = "#8a4600"  # orange[6]
-    green = "#0550ae"  # green[6]
+    red = "#cf222e"  # red[5]
+    orange = "#953800"  # orange[6]
+    green = "#116329"  # green[6]
     blue = "#0550ae"  # blue[6]
     purple = "#8250df"  # purple[5]
     black = "#24292f"  # fg.default
 
 
 class Theme(Style):
     """
-    This style mimics the github light colorblind theme from vscode themes.
+    This style mimics the github light theme from vscode themes.
     """
 
-    default_style = ''
+    default_style = ""
 
     background_color = "#ffffff"  # canvas.default
     highlight_color = "#0969da4a"  # accent.fg
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.red,  # class: 'k'
+        Keyword.Constant: Colors.blue,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.red,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.purple,  # class: 'n'
+        Name.Attribute: Colors.orange,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.green,  # class: 'nt'
+        Name.Variable: Colors.orange,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.blue,  # class: 's'
+        String.Backtick: Colors.blue,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
         # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        Generic.Error: Colors.red,  # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/github_light_high_contrast/style.py` & `accessible_pygments-0.0.5/a11y_pygments/pitaya_smoothie/style.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,106 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#66707b"  # grey[5]
-    red = "#a0111f"  # red[5]
-    orange = "#702c00"  # orange[6]
-    green = "#024c1a"  # green[6]
-    blue = "#023b95"  # blue[6]
-    purple = "#622cbc"  # purple[5]
-    black = "#24292f"  # fg.default
+    comment = "#8786ac"
+    red = "#F26196"
+    orange = "#F5A394"
+    yellow = "#FAD000"
+    green = "#18C1C4"
+    cyan = "#66E9EC"
+    blue = "#7998F2"
+    purple = "#C4A2F5"
+    black = "#FEFEFF"
 
 
 class Theme(Style):
     """
-    This style mimics the github light high contrast theme from vscode themes.
+    This style mimics the a11 light theme from eric bailey's accessible themes.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#ffffff"  # canvas.default
-    highlight_color = "#0969da4a"  # accent.fg
+    background_color = "#181036"
+    highlight_color = "#2A1968"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.comment,  # class: 'c'
-
-        Keyword:                   Colors.red,      # class: 'k'
-        Keyword.Constant:          Colors.blue,     # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.yellow,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.red,      # class: 'kt'
-
-        Operator:                  Colors.green,    # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.purple,   # class: 'n'
-        Name.Attribute:            Colors.orange,   # class: 'na'
-        Name.Builtin:              Colors.orange,   # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.orange,   # class: 'bp'
-        Name.Class:                Colors.blue,     # class: 'nc'
-        Name.Constant:             Colors.blue,     # class: 'no'
-        Name.Decorator:            Colors.orange,   # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.purple,   # class: 'ne'
-        Name.Function:             Colors.blue,     # class: 'nf'
-        Name.Property:             Colors.blue,     # class: 'py'
-        Name.Label:                Colors.orange,   # class: 'nl'
-        Name.Namespace:            Colors.black,    # class: 'nn'
+        Keyword.Type: Colors.orange,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.yellow,  # class: 'na'
+        Name.Builtin: Colors.purple,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.purple,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.blue,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.green,    # class: 'nt'
-        Name.Variable:             Colors.orange,   # class: 'nv'
-        Name.Variable.Magic:       Colors.orange,
+        Name.Tag: Colors.blue,  # class: 'nt'
+        Name.Variable: Colors.orange,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.orange,   # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.orange,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.blue,     # class: 's'
-        String.Backtick:           Colors.blue,     # class: 'sb'
+        String: Colors.blue,  # class: 's'
+        String.Backtick: Colors.cyan,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
-        # String.Doc:                "",            # class: 'sd'
+        String.Doc: Colors.purple,  # class: 'sd'
         # String.Double:             "",            # class: 's2'
-        # String.Escape:             "",            # class: 'se'
+        String.Escape: Colors.orange,  # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.blue,     # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.blue,     # class: 'gd',
-        Generic.Emph:              "italic",        # class: 'ge'
-        Generic.Error:             Colors.red,      # class: 'gr'
-        Generic.Heading:           Colors.blue,     # class: 'gh'
-        Generic.Subheading:        Colors.blue,     # class: 'gu'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
+        # Generic.Error:             "",            # class: 'gr'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/gotthard_dark/style.py` & `accessible_pygments-0.0.5/a11y_pygments/gotthard_light/style.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#F5F5F5"
-    red = "#AB6369"
-    orange = "#B89784"
-    yellow = "#CAAB6D"
-    green = "#81B19B"
-    blue = "#6F98B3"
-    purple = "#b19db4"
-    black = "#F5F5F5"
+    comment = "#141414"
+    red = "#9F4E55"
+    orange = "#A25E53"
+    yellow = "#98661B"
+    green = "#437A6B"
+    blue = "#3D73A9"
+    purple = "#974EB7"
+    black = "#141414"
 
 
 class Theme(Style):
     """
-    This style mimics the gotthard dark theme from vscode.
+    This style mimics the gotthard light theme from vscode.
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#000000"
-    highlight_color = "#4c4b4be8"
+    background_color = "#F5F5F5"
+    highlight_color = "#E1E1E1"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.purple,   # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.red,      # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.purple,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.red,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.green,    # class: 'kt'
-
-        Operator:                  Colors.blue,     # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.purple,   # class: 'na'
-        Name.Builtin:              Colors.green,    # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.green,    # class: 'bp'
-        Name.Class:                Colors.yellow,   # class: 'nc'
-        Name.Constant:             Colors.red,      # class: 'no'
-        Name.Decorator:            Colors.green,    # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.red,      # class: 'ne'
-        Name.Function:             Colors.purple,   # class: 'nf'
-        Name.Property:             Colors.purple,   # class: 'py'
-        Name.Label:                Colors.green,    # class: 'nl'
-        Name.Namespace:            Colors.yellow,   # class: 'nn'
+        Keyword.Type: Colors.green,  # class: 'kt'
+        Operator: Colors.blue,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.purple,  # class: 'na'
+        Name.Builtin: Colors.green,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.green,  # class: 'bp'
+        Name.Class: Colors.yellow,  # class: 'nc'
+        Name.Constant: Colors.red,  # class: 'no'
+        Name.Decorator: Colors.green,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.red,  # class: 'ne'
+        Name.Function: Colors.purple,  # class: 'nf'
+        Name.Property: Colors.purple,  # class: 'py'
+        Name.Label: Colors.green,  # class: 'nl'
+        Name.Namespace: Colors.yellow,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.red,      # class: 'nt'
-        Name.Variable:             Colors.comment,  # class: 'nv'
-        Name.Variable.Magic:       Colors.comment,
+        Name.Tag: Colors.red,  # class: 'nt'
+        Name.Variable: Colors.comment,  # class: 'nv'
+        Name.Variable.Magic: Colors.comment,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.red,      # class: 'm'
+        Number: Colors.red,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.purple,   # class: 'l'
+        Literal: Colors.purple,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.yellow,   # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.yellow,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
-        String.Escape:             Colors.blue,     # class: 'se'
+        String.Escape: Colors.blue,  # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.blue,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.green,    # class: 'ss'
-
+        String.Symbol: Colors.green,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.red,      # class: 'gd',
+        Generic.Deleted: Colors.red,  # class: 'gd',
         # Generic.Emph:              "italic",      # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.green,    # class: 'gh'
-        Generic.Subheading:        Colors.green,    # class: 'gu'
+        Generic.Heading: Colors.green,  # class: 'gh'
+        Generic.Subheading: Colors.green,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

### Comparing `accessible-pygments-0.0.4/a11y_pygments/gotthard_light/style.py` & `accessible_pygments-0.0.5/a11y_pygments/a11y_dark/style.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,107 @@
 from pygments.style import Style
 from pygments.token import (
-    Keyword, Name, Comment, String, Error, Text, Number, Operator, Generic,
-    Punctuation, Other, Literal)
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Text,
+)
 
 
 class Colors:
-    comment = "#141414"
-    red = "#9F4E55"
-    orange = "#A25E53"
-    yellow = "#98661B"
-    green = "#437A6B"
-    blue = "#3D73A9"
-    purple = "#974EB7"
-    black = "#141414"
+    comment = "#d4d0ab"
+    red = "#ffa07a"
+    orange = "#f5ab35"
+    yellow = "#ffd700"
+    green = "#abe338"
+    blue = "#00e0e0"
+    purple = "#dcc6e0"
+    black = "#f8f8f2"
 
 
 class Theme(Style):
     """
-    This style mimics the gotthard light theme from vscode.
+    This is the Pygments implementation of a11y-dark from [Eric Bailey's
+    accessible themes for syntax
+    highlighting](https://github.com/ericwbailey/a11y-syntax-highlighting)
     """
 
-    default_style = ''
+    default_style = ""
 
-    background_color = "#F5F5F5"
-    highlight_color = "#E1E1E1"
+    background_color = "#2b2b2b"
+    highlight_color = "#ffd9002e"
 
     styles = {
-        Text:                      Colors.black,    # class:  ''
-        Error:                     Colors.red,      # class: 'err'
-        Other:                     "",              # class 'x'
-
-        Comment:                   Colors.purple,   # class: 'c'
-
-        Keyword:                   Colors.purple,   # class: 'k'
-        Keyword.Constant:          Colors.red,      # class: 'kc'
+        Text: Colors.black,  # class:  ''
+        Error: Colors.red,  # class: 'err'
+        Other: "",  # class 'x'
+        Comment: Colors.comment,  # class: 'c'
+        Keyword: Colors.purple,  # class: 'k'
+        Keyword.Constant: Colors.purple,  # class: 'kc'
         # Keyword.Declaration:       "",            # class: 'kd'
         # Keyword.Namespace:         "",            # class: 'kn'
         # Keyword.Pseudo:            "",            # class: 'kp'
         # Keyword.Reserved:          "",            # class: 'kr'
-        Keyword.Type:              Colors.green,    # class: 'kt'
-
-        Operator:                  Colors.blue,     # class: 'o'
-        Operator.Word:             Colors.purple,   # class: 'ow'
-
-        Punctuation:               Colors.black,    # class: 'p'
-
-        Name:                      Colors.black,    # class: 'n'
-        Name.Attribute:            Colors.purple,   # class: 'na'
-        Name.Builtin:              Colors.green,    # class: 'nb'
-        Name.Builtin.Pseudo:       Colors.green,    # class: 'bp'
-        Name.Class:                Colors.yellow,   # class: 'nc'
-        Name.Constant:             Colors.red,      # class: 'no'
-        Name.Decorator:            Colors.green,    # class: 'nd'
-        Name.Entity:               Colors.green,    # class: 'ni'
-        Name.Exception:            Colors.red,      # class: 'ne'
-        Name.Function:             Colors.purple,   # class: 'nf'
-        Name.Property:             Colors.purple,   # class: 'py'
-        Name.Label:                Colors.green,    # class: 'nl'
-        Name.Namespace:            Colors.yellow,   # class: 'nn'
+        Keyword.Type: Colors.orange,  # class: 'kt'
+        Operator: Colors.green,  # class: 'o'
+        Operator.Word: Colors.purple,  # class: 'ow'
+        Punctuation: Colors.black,  # class: 'p'
+        Name: Colors.black,  # class: 'n'
+        Name.Attribute: Colors.yellow,  # class: 'na'
+        Name.Builtin: Colors.orange,  # class: 'nb'
+        Name.Builtin.Pseudo: Colors.orange,  # class: 'bp'
+        Name.Class: Colors.blue,  # class: 'nc'
+        Name.Constant: Colors.blue,  # class: 'no'
+        Name.Decorator: Colors.orange,  # class: 'nd'
+        Name.Entity: Colors.green,  # class: 'ni'
+        Name.Exception: Colors.purple,  # class: 'ne'
+        Name.Function: Colors.blue,  # class: 'nf'
+        Name.Property: Colors.blue,  # class: 'py'
+        Name.Label: Colors.orange,  # class: 'nl'
+        Name.Namespace: Colors.black,  # class: 'nn'
         # Name.Other:                "",            # class: 'nx'
-        Name.Tag:                  Colors.red,      # class: 'nt'
-        Name.Variable:             Colors.comment,  # class: 'nv'
-        Name.Variable.Magic:       Colors.comment,
+        Name.Tag: Colors.blue,  # class: 'nt'
+        Name.Variable: Colors.red,  # class: 'nv'
+        Name.Variable.Magic: Colors.orange,
         # Name.Variable.Class:       "",            # class: 'vc'
         # Name.Variable.Global:      "",            # class: 'vg'
         # Name.Variable.Instance:    "",            # class: 'vi'
-
-        Number:                    Colors.red,      # class: 'm'
+        Number: Colors.orange,  # class: 'm'
         # Number.Float:              "",            # class: 'mf'
         # Number.Hex:                "",            # class: 'mh'
         # Number.Integer:            "",            # class: 'mi'
         # Number.Integer.Long:       "",            # class: 'il'
         # Number.Oct:                "",            # class: 'mo'
-
-        Literal:                   Colors.purple,   # class: 'l'
+        Literal: Colors.orange,  # class: 'l'
         # Literal.Date:              "",            # class: 'ld'
-
-        String:                    Colors.green,    # class: 's'
-        String.Backtick:           Colors.yellow,   # class: 'sb'
+        String: Colors.green,  # class: 's'
+        String.Backtick: Colors.green,  # class: 'sb'
         # String.Char:               "",            # class: 'sc'
         # String.Doc:                "",            # class: 'sd'
         # String.Double:             "",            # class: 's2'
-        String.Escape:             Colors.blue,     # class: 'se'
+        # String.Escape:             "",            # class: 'se'
         # String.Heredoc:            "",            # class: 'sh'
         # String.Interpol:           "",            # class: 'si'
         # String.Other:              "",            # class: 'sx'
-        String.Regex:              Colors.blue,     # class: 'sr'
+        String.Regex: Colors.red,  # class: 'sr'
         # String.Single:             "",            # class: 's1'
-        String.Symbol:             Colors.green,    # class: 'ss'
-
+        String.Symbol: Colors.blue,  # class: 'ss'
         # Generic:                   "",            # class: 'g'
-        Generic.Deleted:           Colors.red,      # class: 'gd',
-        # Generic.Emph:              "italic",      # class: 'ge'
+        Generic.Deleted: Colors.blue,  # class: 'gd',
+        Generic.Emph: "italic",  # class: 'ge'
         # Generic.Error:             "",            # class: 'gr'
-        Generic.Heading:           Colors.green,    # class: 'gh'
-        Generic.Subheading:        Colors.green,    # class: 'gu'
+        Generic.Heading: Colors.blue,  # class: 'gh'
+        Generic.Subheading: Colors.blue,  # class: 'gu'
         # Generic.Inserted:          "",            # class: 'gi'
         # Generic.Output:            "",            # class: 'go'
         # Generic.Prompt:            "",            # class: 'gp'
-        Generic.Strong:            "bold",          # class: 'gs'
+        Generic.Strong: "bold",  # class: 'gs'
         # Generic.Traceback:         "",            # class: 'gt'
-    }
+    }
```

