# Comparing `tmp/delf-0.1.3.tar.gz` & `tmp/delf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delf-0.1.3.tar", max compression
+gzip compressed data, was "delf-0.1.4.tar", max compression
```

## Comparing `delf-0.1.3.tar` & `delf-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2022-03-03 04:30:48.399678 delf-0.1.3/LICENSE
--rw-r--r--   0        0        0     2751 2023-11-09 01:16:07.830869 delf-0.1.3/README.md
--rw-r--r--   0        0        0      649 2023-12-04 22:55:45.979178 delf-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0    74409 2023-10-22 15:01:59.198220 delf-0.1.3/src/delf.py
--rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 delf-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-03-03 04:30:48.399678 delf-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2595 2023-12-04 22:57:37.645182 delf-0.1.4/README.md
+-rw-r--r--   0        0        0      672 2024-05-09 22:10:08.702014 delf-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0    74409 2023-10-22 15:01:59.198220 delf-0.1.4/src/delf.py
+-rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 delf-0.1.4/PKG-INFO
```

### Comparing `delf-0.1.3/LICENSE` & `delf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `delf-0.1.3/README.md` & `delf-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/bloodstalker/delf.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/bloodstalker/delf/alerts/)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/fe73b673bf0343aeae1c84ff1911b3ce)](https://www.codacy.com/gh/terminaldweller/delf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=terminaldweller/delf&amp;utm_campaign=Badge_Grade)
 
 # delf
 delf is an ELF dump tool.<br/>
 
 ## Installation
 You will also need to have `libcapstone` installed.
```

### Comparing `delf-0.1.3/pyproject.toml` & `delf-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delf"
-version = "0.1.3"
+version = "0.1.4"
 description = "yet another elf dump tool"
 authors = ["terminaldweller <devi@terminaldweller.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 keywords = ["elf", "capstone"]
 classifiers = [
     "Environment :: Console",
@@ -12,14 +12,15 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 capstone = "^4.0.2"
+setuptools = "^69.5.1"
 
 [tool.poetry.scripts]
 delf = "delf:main"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `delf-0.1.3/src/delf.py` & `delf-0.1.4/src/delf.py`

 * *Files identical despite different names*

### Comparing `delf-0.1.3/PKG-INFO` & `delf-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: delf
-Version: 0.1.3
+Version: 0.1.4
 Summary: yet another elf dump tool
 License: GPL-3.0
 Keywords: elf,capstone
 Author: terminaldweller
 Author-email: devi@terminaldweller.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: capstone (>=4.0.2,<5.0.0)
+Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Description-Content-Type: text/markdown
 
 
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/bloodstalker/delf.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/bloodstalker/delf/alerts/)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/fe73b673bf0343aeae1c84ff1911b3ce)](https://www.codacy.com/gh/terminaldweller/delf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=terminaldweller/delf&amp;utm_campaign=Badge_Grade)
 
 # delf
 delf is an ELF dump tool.<br/>
 
 ## Installation
 You will also need to have `libcapstone` installed.
```

