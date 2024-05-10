# Comparing `tmp/jzchatbot-59.83.89.tar.gz` & `tmp/jzchatbot-59.83.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.89.tar", last modified: Thu May  9 03:31:36 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.90.tar", last modified: Fri May 10 01:35:08 2024, max compression
```

## Comparing `jzchatbot-59.83.89.tar` & `jzchatbot-59.83.90.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.140287 jzchatbot-59.83.89/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.89/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-09 03:31:36.137669 jzchatbot-59.83.89/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.89/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.099199 jzchatbot-59.83.89/jzchatbot/
--rw-rw-rw-   0        0        0     2441 2024-05-09 03:31:14.000000 jzchatbot-59.83.89/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:31:36.132777 jzchatbot-59.83.89/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 03:31:35.000000 jzchatbot-59.83.89/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 03:31:36.140287 jzchatbot-59.83.89/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-09 03:26:03.000000 jzchatbot-59.83.89/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.238433 jzchatbot-59.83.90/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.90/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-10 01:35:08.231270 jzchatbot-59.83.90/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 01:15:53.000000 jzchatbot-59.83.90/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.195824 jzchatbot-59.83.90/jzchatbot/
+-rw-rw-rw-   0        0        0     4111 2024-05-10 01:33:48.000000 jzchatbot-59.83.90/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:35:08.231270 jzchatbot-59.83.90/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-10 01:35:08.000000 jzchatbot-59.83.90/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 01:35:07.000000 jzchatbot-59.83.90/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 01:35:08.239445 jzchatbot-59.83.90/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-10 01:34:57.000000 jzchatbot-59.83.90/setup.py
```

### Comparing `jzchatbot-59.83.89/LICENSE` & `jzchatbot-59.83.90/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.89/setup.py` & `jzchatbot-59.83.90/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.89", 
+	version="59.83.90", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

