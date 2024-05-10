# Comparing `tmp/hebill_html-1.0.0.tar.gz` & `tmp/hebill_html-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill_html-1.0.0.tar", last modified: Thu May  9 02:52:16 2024, max compression
+gzip compressed data, was "hebill_html-1.0.1.tar", last modified: Fri May 10 03:12:07 2024, max compression
```

## Comparing `hebill_html-1.0.0.tar` & `hebill_html-1.0.1.tar`

### file list

```diff
@@ -1,161 +1,173 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.502171 hebill_html-1.0.0/
--rw-rw-rw-   0        0        0     1301 2024-05-09 02:52:16.501115 hebill_html-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.347673 hebill_html-1.0.0/hebill_html/
--rw-rw-rw-   0        0        0     1095 2024-05-09 02:49:52.000000 hebill_html-1.0.0/hebill_html/README.MD
--rw-rw-rw-   0        0        0      121 2024-05-09 02:49:03.000000 hebill_html-1.0.0/hebill_html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.392549 hebill_html-1.0.0/hebill_html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.396398 hebill_html-1.0.0/hebill_html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill_html-1.0.0/hebill_html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.404404 hebill_html-1.0.0/hebill_html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill_html-1.0.0/hebill_html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill_html-1.0.0/hebill_html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill_html-1.0.0/hebill_html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.410386 hebill_html-1.0.0/hebill_html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill_html-1.0.0/hebill_html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill_html-1.0.0/hebill_html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.413374 hebill_html-1.0.0/hebill_html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill_html-1.0.0/hebill_html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.418008 hebill_html-1.0.0/hebill_html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill_html-1.0.0/hebill_html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill_html-1.0.0/hebill_html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.420134 hebill_html-1.0.0/hebill_html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill_html-1.0.0/hebill_html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill_html-1.0.0/hebill_html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.423610 hebill_html-1.0.0/hebill_html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.427597 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.438431 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill_html-1.0.0/hebill_html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.442632 hebill_html-1.0.0/hebill_html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill_html-1.0.0/hebill_html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill_html-1.0.0/hebill_html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.443629 hebill_html-1.0.0/hebill_html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill_html-1.0.0/hebill_html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.445110 hebill_html-1.0.0/hebill_html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill_html-1.0.0/hebill_html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      306 2024-05-09 02:49:03.000000 hebill_html-1.0.0/hebill_html/constants.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill_html-1.0.0/hebill_html/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.446111 hebill_html-1.0.0/hebill_html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.449464 hebill_html-1.0.0/hebill_html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill_html-1.0.0/hebill_html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill_html-1.0.0/hebill_html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.450476 hebill_html-1.0.0/hebill_html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill_html-1.0.0/hebill_html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill_html-1.0.0/hebill_html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.451978 hebill_html-1.0.0/hebill_html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill_html-1.0.0/hebill_html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill_html-1.0.0/hebill_html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.453489 hebill_html-1.0.0/hebill_html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill_html-1.0.0/hebill_html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill_html-1.0.0/hebill_html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.454498 hebill_html-1.0.0/hebill_html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.457524 hebill_html-1.0.0/hebill_html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.458521 hebill_html-1.0.0/hebill_html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.460514 hebill_html-1.0.0/hebill_html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill_html-1.0.0/hebill_html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.462507 hebill_html-1.0.0/hebill_html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill_html-1.0.0/hebill_html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill_html-1.0.0/hebill_html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.465497 hebill_html-1.0.0/hebill_html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill_html-1.0.0/hebill_html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.466997 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.467998 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.468999 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill_html-1.0.0/hebill_html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill_html-1.0.0/hebill_html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.470130 hebill_html-1.0.0/hebill_html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.471131 hebill_html-1.0.0/hebill_html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill_html-1.0.0/hebill_html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.472450 hebill_html-1.0.0/hebill_html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill_html-1.0.0/hebill_html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.473453 hebill_html-1.0.0/hebill_html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill_html-1.0.0/hebill_html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.474449 hebill_html-1.0.0/hebill_html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.475446 hebill_html-1.0.0/hebill_html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.476443 hebill_html-1.0.0/hebill_html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.479543 hebill_html-1.0.0/hebill_html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.480539 hebill_html-1.0.0/hebill_html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.482787 hebill_html-1.0.0/hebill_html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.0/hebill_html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.484287 hebill_html-1.0.0/hebill_html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill_html-1.0.0/hebill_html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.485800 hebill_html-1.0.0/hebill_html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill_html-1.0.0/hebill_html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.486797 hebill_html-1.0.0/hebill_html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill_html-1.0.0/hebill_html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.488303 hebill_html-1.0.0/hebill_html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill_html-1.0.0/hebill_html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.489316 hebill_html-1.0.0/hebill_html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill_html-1.0.0/hebill_html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.490810 hebill_html-1.0.0/hebill_html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill_html-1.0.0/hebill_html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.491810 hebill_html-1.0.0/hebill_html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill_html-1.0.0/hebill_html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.493804 hebill_html-1.0.0/hebill_html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill_html-1.0.0/hebill_html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.494801 hebill_html-1.0.0/hebill_html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill_html-1.0.0/hebill_html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.496130 hebill_html-1.0.0/hebill_html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill_html-1.0.0/hebill_html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.497123 hebill_html-1.0.0/hebill_html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill_html-1.0.0/hebill_html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.498125 hebill_html-1.0.0/hebill_html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill_html-1.0.0/hebill_html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.500118 hebill_html-1.0.0/hebill_html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill_html-1.0.0/hebill_html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill_html-1.0.0/hebill_html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:52:16.501115 hebill_html-1.0.0/hebill_html.egg-info/
--rw-rw-rw-   0        0        0     1301 2024-05-09 02:52:16.000000 hebill_html-1.0.0/hebill_html.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3902 2024-05-09 02:52:16.000000 hebill_html-1.0.0/hebill_html.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:52:16.000000 hebill_html-1.0.0/hebill_html.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 02:52:16.000000 hebill_html-1.0.0/hebill_html.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      485 2024-05-09 02:52:15.000000 hebill_html-1.0.0/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-05-09 02:52:16.502171 hebill_html-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.861299 hebill_html-1.0.1/
+-rw-rw-rw-   0        0        0      210 2024-05-10 03:12:07.859305 hebill_html-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.677117 hebill_html-1.0.1/hebill_html/
+-rw-rw-rw-   0        0        0       50 2024-05-09 02:55:17.000000 hebill_html-1.0.1/hebill_html/README.MD
+-rw-rw-rw-   0        0        0      121 2024-05-09 02:49:03.000000 hebill_html-1.0.1/hebill_html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.689098 hebill_html-1.0.1/hebill_html/components/
+-rw-rw-rw-   0        0        0       91 2024-05-10 02:47:48.000000 hebill_html-1.0.1/hebill_html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.691552 hebill_html-1.0.1/hebill_html/components/alert/
+-rw-rw-rw-   0        0        0        0 2024-05-10 02:38:54.000000 hebill_html-1.0.1/hebill_html/components/alert/__init__.py
+-rw-rw-rw-   0        0        0      867 2024-05-10 02:42:23.000000 hebill_html-1.0.1/hebill_html/components/alert/color.py
+-rw-rw-rw-   0        0        0      394 2024-05-10 02:42:23.000000 hebill_html-1.0.1/hebill_html/components/alert/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.692552 hebill_html-1.0.1/hebill_html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill_html-1.0.1/hebill_html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.693551 hebill_html-1.0.1/hebill_html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill_html-1.0.1/hebill_html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-09 07:14:12.000000 hebill_html-1.0.1/hebill_html/components/html/body/core.py
+-rw-rw-rw-   0        0        0     2325 2024-05-09 08:49:57.000000 hebill_html-1.0.1/hebill_html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.695189 hebill_html-1.0.1/hebill_html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill_html-1.0.1/hebill_html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      660 2024-05-09 07:38:50.000000 hebill_html-1.0.1/hebill_html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.696289 hebill_html-1.0.1/hebill_html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill_html-1.0.1/hebill_html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.697291 hebill_html-1.0.1/hebill_html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill_html-1.0.1/hebill_html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      448 2024-05-09 07:04:46.000000 hebill_html-1.0.1/hebill_html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.700548 hebill_html-1.0.1/hebill_html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill_html-1.0.1/hebill_html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      867 2024-05-10 01:35:59.000000 hebill_html-1.0.1/hebill_html/components/table/color.py
+-rw-rw-rw-   0        0        0     2388 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.701922 hebill_html-1.0.1/hebill_html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0     1065 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.705166 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      875 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.708156 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-10 01:34:25.000000 hebill_html-1.0.1/hebill_html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.710662 hebill_html-1.0.1/hebill_html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill_html-1.0.1/hebill_html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0     1065 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.714164 hebill_html-1.0.1/hebill_html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      875 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.717690 hebill_html-1.0.1/hebill_html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-10 01:34:25.000000 hebill_html-1.0.1/hebill_html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      306 2024-05-10 03:12:06.000000 hebill_html-1.0.1/hebill_html/constants.py
+-rw-rw-rw-   0        0        0      966 2024-05-09 03:06:16.000000 hebill_html-1.0.1/hebill_html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.720194 hebill_html-1.0.1/hebill_html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.725684 hebill_html-1.0.1/hebill_html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill_html-1.0.1/hebill_html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill_html-1.0.1/hebill_html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.728686 hebill_html-1.0.1/hebill_html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill_html-1.0.1/hebill_html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill_html-1.0.1/hebill_html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.732673 hebill_html-1.0.1/hebill_html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill_html-1.0.1/hebill_html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-05-09 07:38:50.000000 hebill_html-1.0.1/hebill_html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.736660 hebill_html-1.0.1/hebill_html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill_html-1.0.1/hebill_html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0     1242 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.738987 hebill_html-1.0.1/hebill_html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.747359 hebill_html-1.0.1/hebill_html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-05-10 02:47:48.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.755411 hebill_html-1.0.1/hebill_html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.765902 hebill_html-1.0.1/hebill_html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2611 2024-05-09 07:54:39.000000 hebill_html-1.0.1/hebill_html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.768891 hebill_html-1.0.1/hebill_html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill_html-1.0.1/hebill_html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.771881 hebill_html-1.0.1/hebill_html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill_html-1.0.1/hebill_html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.774871 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.776865 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0     1264 2024-05-10 00:45:38.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1647 2024-05-09 07:44:11.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.779365 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill_html-1.0.1/hebill_html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1223 2024-05-09 03:35:01.000000 hebill_html-1.0.1/hebill_html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.790906 hebill_html-1.0.1/hebill_html/tags/
+-rw-rw-rw-   0        0        0      673 2024-05-10 03:08:59.000000 hebill_html-1.0.1/hebill_html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.794403 hebill_html-1.0.1/hebill_html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill_html-1.0.1/hebill_html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      320 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.799290 hebill_html-1.0.1/hebill_html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill_html-1.0.1/hebill_html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.803421 hebill_html-1.0.1/hebill_html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill_html-1.0.1/hebill_html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.805413 hebill_html-1.0.1/hebill_html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.807912 hebill_html-1.0.1/hebill_html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.811410 hebill_html-1.0.1/hebill_html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.820893 hebill_html-1.0.1/hebill_html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 01:59:38.000000 hebill_html-1.0.1/hebill_html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.823817 hebill_html-1.0.1/hebill_html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.824826 hebill_html-1.0.1/hebill_html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill_html-1.0.1/hebill_html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.827817 hebill_html-1.0.1/hebill_html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill_html-1.0.1/hebill_html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.829319 hebill_html-1.0.1/hebill_html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill_html-1.0.1/hebill_html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      303 2024-05-09 08:46:30.000000 hebill_html-1.0.1/hebill_html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.831316 hebill_html-1.0.1/hebill_html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill_html-1.0.1/hebill_html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.832313 hebill_html-1.0.1/hebill_html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill_html-1.0.1/hebill_html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.834306 hebill_html-1.0.1/hebill_html/tags/meta/
+-rw-rw-rw-   0        0        0        0 2024-05-09 03:11:25.000000 hebill_html-1.0.1/hebill_html/tags/meta/__init__.py
+-rw-rw-rw-   0        0        0      432 2024-05-09 03:39:59.000000 hebill_html-1.0.1/hebill_html/tags/meta/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.836300 hebill_html-1.0.1/hebill_html/tags/nav/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill_html-1.0.1/hebill_html/tags/nav/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-05-10 03:08:59.000000 hebill_html-1.0.1/hebill_html/tags/nav/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.838369 hebill_html-1.0.1/hebill_html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill_html-1.0.1/hebill_html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.839393 hebill_html-1.0.1/hebill_html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill_html-1.0.1/hebill_html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      206 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.841418 hebill_html-1.0.1/hebill_html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill_html-1.0.1/hebill_html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.843502 hebill_html-1.0.1/hebill_html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill_html-1.0.1/hebill_html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.844657 hebill_html-1.0.1/hebill_html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill_html-1.0.1/hebill_html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.846663 hebill_html-1.0.1/hebill_html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill_html-1.0.1/hebill_html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.848081 hebill_html-1.0.1/hebill_html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill_html-1.0.1/hebill_html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.849092 hebill_html-1.0.1/hebill_html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill_html-1.0.1/hebill_html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      437 2024-05-10 02:27:12.000000 hebill_html-1.0.1/hebill_html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.851100 hebill_html-1.0.1/hebill_html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill_html-1.0.1/hebill_html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill_html-1.0.1/hebill_html/tags/tr/core.py
+-rw-rw-rw-   0        0        0      518 2024-05-10 00:45:38.000000 hebill_html-1.0.1/hebill_html/tpl_style.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:12:07.852798 hebill_html-1.0.1/hebill_html.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-05-10 03:12:07.000000 hebill_html-1.0.1/hebill_html.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4207 2024-05-10 03:12:07.000000 hebill_html-1.0.1/hebill_html.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:12:07.000000 hebill_html-1.0.1/hebill_html.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 03:12:07.000000 hebill_html-1.0.1/hebill_html.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      485 2024-05-10 03:12:06.000000 hebill_html-1.0.1/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:12:07.861299 hebill_html-1.0.1/setup.cfg
```

### Comparing `hebill_html-1.0.0/hebill_html/components/table/tbody/core.py` & `hebill_html-1.0.1/hebill_html/nodes/group/create/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from ....tags.tbody.core import Tbody as TbodyParentClass
-from .tr.core import Tr
-
-
-class Tbody(TbodyParentClass):
-    def __init__(self, senior):
-        super().__init__(senior)
-        self._rows = []
-        self._row = None
+class Create:
+    def __init__(self, sir):
+        self.senior = sir
+        self._nodes = None
+        self._tags = None
+        self._components = None
 
     @property
-    def rows(self) -> list:
-        return self._rows
+    def node(self):
+        if self._nodes is None:
+            from .nodes.core import Nodes
+            self._nodes = Nodes(self.senior)
+        return self._nodes
 
     @property
-    def row(self) -> Tr:
-        if self._row is None:
-            self.add_row()
-        return self._row
+    def tag(self):
+        if self._tags is None:
+            from .tags.core import Tags
+            self._tags = Tags(self.senior)
+        return self._tags
 
-    def add_row(self) -> Tr:
-        self._row = Tr(self)
-        self._rows.append(self._row)
-        return self._row
+    @property
+    def component(self):
+        if self._components is None:
+            from .components.core import Components
+            self._components = Components(self.senior)
+        return self._components
```

### Comparing `hebill_html-1.0.0/hebill_html/components/table/thead/core.py` & `hebill_html-1.0.1/hebill_html/components/table/thead/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,21 +4,41 @@
 
 class Thead(TheadParentClass):
     def __init__(self, senior):
         super().__init__(senior)
         self._rows = []
         self._row = None
 
+        self._style = None
+
     @property
     def rows(self) -> list:
         return self._rows
 
     @property
     def row(self) -> Tr:
         if self._row is None:
             self.add_row()
         return self._row
 
-    def add_row(self) -> Tr:
+    @property
+    def cells(self): return self.row.cells
+
+    @property
+    def cell(self): return self.row.cell
+
+    def add_cell(self, text=None): return self.row.add_cell(text)
+
+    def add_row(self, data: list = None) -> Tr:
         self._row = Tr(self)
         self._rows.append(self._row)
+        if data:
+            for d in data:
+                self.row.add_cell(d)
         return self._row
+
+    @property
+    def color(self):
+        if self._style is None:
+            from ..color import Color
+            self._style = Color(self)
+        return self._style
```

### Comparing `hebill_html-1.0.0/hebill_html/core.py` & `hebill_html-1.0.1/hebill_html/core.py`

 * *Files identical despite different names*

### Comparing `hebill_html-1.0.0/hebill_html/nodes/comment/core.py` & `hebill_html-1.0.1/hebill_html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill_html-1.0.0/hebill_html/nodes/group/core.py` & `hebill_html-1.0.1/hebill_html/components/html/head/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from ..node.core import Node
+from ....tags.head.core import Head as HeadParentClass
+from .title.core import Title
 
 
-class Group(Node):
-    def __init__(self, sir):
-        super().__init__(sir)
-        self._juniors = {}
-        self._create = None
+class Head(HeadParentClass):
+    def __init__(self, senior):
+        super().__init__(senior)
+        self._metas = self.create.node.group()
+        self._title = self.create.tag.title()
+        self._libraries = self.create.node.group()
 
     @property
-    def juniors(self): return self._juniors
+    def metas(self):
+        return self._metas.create.tag.title()
 
-    def local_add_junior(self, jun: Node): self._juniors[jun.id] = jun
-
-    def has_juniors(self): return len(self._juniors) > 0
+    @property
+    def libraries(self):
+        return self._libraries
 
     @property
-    def create(self):
-        if self._create is None:
-            from .create.core import Create
-            self._create = Create(self)
-        return self._create
-
-    def output(self):
-        s = ""
-        if self.has_juniors():
-            for key, value in self.juniors.items():
-                s += value.output()
-        return s
+    def title(self):
+        return self._title.content
+
+    @title.setter
+    def title(self, title):
+        self._title.content = title
+
```

### Comparing `hebill_html-1.0.0/hebill_html/nodes/group/create/nodes/core.py` & `hebill_html-1.0.1/hebill_html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill_html-1.0.0/hebill_html/nodes/group/create/tags/core.py` & `hebill_html-1.0.1/hebill_html/nodes/group/create/tags/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         from .....tags import InputText
         return InputText(self.senior, name, value, placeholder)
 
     def link(self, url: str = None):
         from .....tags import Link
         return Link(self.senior, url)
 
+    def meta(self):
+        from .....tags import Meta
+        return Meta(self.senior)
+
     def script(self, url: str = None):
         from .....tags import Script
         return Script(self.senior, url)
 
     def span(self, text: str = None):
         from .....tags import Span
         return Span(self.senior, text)
```

### Comparing `hebill_html-1.0.0/hebill_html/nodes/node/core.py` & `hebill_html-1.0.1/hebill_html/nodes/node/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
     @property
     def document(self): return self._document
 
     @property
     def senior(self): return self._senior
 
+    def local_change_senior(self, sir):
+        self.senior.local_remove_junior(self)
+        self._senior = sir
+
     @property
     def level(self) -> int:
         if self._senior is None:
             return 0
         from ...nodes.tag.core import Tag
         from ...nodes.group.core import Group
         if isinstance(self, Group) and not isinstance(self, Tag):
```

### Comparing `hebill_html-1.0.0/hebill_html/nodes/tag/attributes/classes/core.py` & `hebill_html-1.0.1/hebill_html/nodes/tag/attributes/classes/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,38 @@
     def reset(self, classes: str | list = None) -> bool:
         self.clear()
         if classes is None:
             return True
         return self.set(classes)
 
     def set(self, classes: str | list = None) -> bool:
-        if classes is None:
-            return False
         if isinstance(classes, str):
-            self.extend(classes.split(' '))
+            if ' ' in classes:
+                self.set(classes.split(' '))
+            else:
+                if classes not in self:
+                    self.append(classes)
+            return True
+        elif isinstance(classes, list):
+            for c in classes:
+                self.set(c)
+            return True
+        return False
+
+    def unset(self, classes: str | list = None) -> bool:
+        if isinstance(classes, str):
+            if ' ' in classes:
+                self.unset(classes.split(' '))
+            else:
+                if classes in self:
+                    self.remove(classes)
             return True
         elif isinstance(classes, list):
-            self.extend(classes)
+            for c in classes:
+                self.unset(c)
             return True
         return False
 
     @property
     def is_empty(self) -> bool: return len(self) <= 0
 
     def __str__(self): return ' '.join(self)
```

### Comparing `hebill_html-1.0.0/hebill_html/nodes/tag/attributes/core.py` & `hebill_html-1.0.1/hebill_html/nodes/tag/attributes/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,33 +16,41 @@
             super().__setitem__(key, '')
         elif key == 'style':
             self.styles.set(value)
             print('验证styles' + value)
             super().__setitem__(key, '')
         else:
             super().__setitem__(key, value)
-        
+
     def __getitem__(self, key):
         key = key.lower()
         if key == 'class':
             return self.classes.output()
         elif key == 'style':
             return self.styles.output()
         else:
             return super().__getitem__(key)
 
-    def is_empty(self) -> bool: return self.classes.is_empty and self.styles.is_empty and len(self) <= 0
+    def is_empty(self) -> bool:
+        return self.classes.is_empty and self.styles.is_empty and len(self) <= 0
 
     @property
-    def classes(self): return self._classes
+    def classes(self):
+        return self._classes
 
     @property
-    def styles(self): return self._styles
+    def styles(self):
+        return self._styles
 
     def __str__(self):
         if len(self.classes) > 0:
             super().__setitem__('class', self.classes.output())
         if len(self.styles) > 0:
             super().__setitem__('style', self.styles.output())
         return ''.join(f" {n}=\"{v}\"" for n, v in self.items())
 
-    def output(self) -> str: return self.__str__()
+    def add(self, name: str, value: str):
+        if name:
+            self[name] = value
+
+    def output(self) -> str:
+        return self.__str__()
```

### Comparing `hebill_html-1.0.0/hebill_html/nodes/tag/attributes/styles/core.py` & `hebill_html-1.0.1/hebill_html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill_html-1.0.0/hebill_html/nodes/tag/core.py` & `hebill_html-1.0.1/hebill_html/nodes/tag/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class Tag(Group):
     def __init__(self, sir, tag):
         super().__init__(sir)
         self._tag = tag
         from .attributes.core import Attributes
         self._attributes = Attributes()
         self.output_breakable = True
+        self.output_paired = True
 
     @property
     def tag(self): return self._tag
 
     @property
     def attributes(self): return self._attributes
 
@@ -21,14 +22,16 @@
             if self.output_breakable and self.document.output_next_breakable:
                 if self.level > 0:
                     s += "\n"
             s += self.document.output_retraction * self.level
         s += "<" + self.tag
         s += self.attributes.output()
         s += ">"
+        if not self.output_paired:
+            return s
         self.document.output_next_breakable = True
         si = super().output()
         s += si
         if self.document.output_break:
             if si != "" and self.document.output_next_breakable:
                 s += "\n" + "	" * self.level
         s += "</" + self.tag + ">"
```

### Comparing `hebill_html-1.0.0/hebill_html/tags/__init__.py` & `hebill_html-1.0.1/hebill_html/tags/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from .h4.core import H4
 from .h5.core import H5
 from .h6.core import H6
 from .head.core import Head
 from .html.core import Html
 from .input_text.core import InputText
 from .link.core import Link
+from .meta.core import Meta
+from .nav.core import Nav
 from .script.core import Script
 from .span.core import Span
 from .table.core import Table
 from .tbody.core import Tbody
 from .td.core import Td
 from .th.core import Th
 from .thead.core import Thead
```

### Comparing `hebill_html-1.0.0/hebill_html.egg-info/SOURCES.txt` & `hebill_html-1.0.1/hebill_html.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 pack_upload_setup.py
 hebill_html/README.MD
 hebill_html/__init__.py
 hebill_html/constants.py
 hebill_html/core.py
+hebill_html/tpl_style.py
 hebill_html.egg-info/PKG-INFO
 hebill_html.egg-info/SOURCES.txt
 hebill_html.egg-info/dependency_links.txt
 hebill_html.egg-info/top_level.txt
 hebill_html/components/__init__.py
+hebill_html/components/alert/__init__.py
+hebill_html/components/alert/color.py
+hebill_html/components/alert/core.py
 hebill_html/components/html/__init__.py
 hebill_html/components/html/core.py
 hebill_html/components/html/body/__init__.py
 hebill_html/components/html/body/core.py
 hebill_html/components/html/head/__init__.py
 hebill_html/components/html/head/core.py
 hebill_html/components/html/head/title/__init__.py
 hebill_html/components/html/head/title/core.py
 hebill_html/components/html/libraries/__init__.py
 hebill_html/components/html/libraries/libraries.py
 hebill_html/components/table/__init__.py
+hebill_html/components/table/color.py
 hebill_html/components/table/core.py
 hebill_html/components/table/tbody/__init__.py
 hebill_html/components/table/tbody/core.py
 hebill_html/components/table/tbody/tr/__init__.py
 hebill_html/components/table/tbody/tr/core.py
 hebill_html/components/table/tbody/tr/td/__init__.py
 hebill_html/components/table/tbody/tr/td/core.py
@@ -82,14 +87,18 @@
 hebill_html/tags/head/core.py
 hebill_html/tags/html/__init__.py
 hebill_html/tags/html/core.py
 hebill_html/tags/input_text/__init__.py
 hebill_html/tags/input_text/core.py
 hebill_html/tags/link/__init__.py
 hebill_html/tags/link/core.py
+hebill_html/tags/meta/__init__.py
+hebill_html/tags/meta/core.py
+hebill_html/tags/nav/__init__.py
+hebill_html/tags/nav/core.py
 hebill_html/tags/script/__init__.py
 hebill_html/tags/script/core.py
 hebill_html/tags/span/__init__.py
 hebill_html/tags/span/core.py
 hebill_html/tags/table/__init__.py
 hebill_html/tags/table/core.py
 hebill_html/tags/tbody/__init__.py
```

