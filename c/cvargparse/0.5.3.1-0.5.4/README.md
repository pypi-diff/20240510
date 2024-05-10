# Comparing `tmp/cvargparse-0.5.3.1.tar.gz` & `tmp/cvargparse-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvargparse-0.5.3.1.tar", last modified: Thu Mar  7 12:24:50 2024, max compression
+gzip compressed data, was "cvargparse-0.5.4.tar", last modified: Fri May 10 09:36:16 2024, max compression
```

## Comparing `cvargparse-0.5.3.1.tar` & `cvargparse-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/
--rw-r--r--   0 korsch    (1000) korsch    (1000)      233 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/PKG-INFO
--rw-r--r--   0 korsch    (1000) korsch    (1000)     3678 2024-03-07 12:24:10.000000 cvargparse-0.5.3.1/README.md
-drwxr-xr-x   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/cvargparse/
--rw-r--r--   0 korsch    (1000) korsch    (1000)      950 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/__init__.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)       24 2024-03-07 12:24:26.000000 cvargparse-0.5.3.1/cvargparse/_version.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)      877 2024-03-07 12:24:10.000000 cvargparse-0.5.3.1/cvargparse/argument.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)     1428 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/factory.py
-drwxr-xr-x   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/cvargparse/parser/
--rw-r--r--   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/parser/__init__.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)     4325 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/parser/base.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)      262 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/parser/gpu_parser.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)      978 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/parser/mode_parser.py
-drwxr-xr-x   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/cvargparse/utils/
--rw-r--r--   0 korsch    (1000) korsch    (1000)      151 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/utils/__init__.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)     2963 2024-03-07 12:24:10.000000 cvargparse-0.5.3.1/cvargparse/utils/dataclass.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)      208 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/utils/decorators.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)     1497 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/utils/enumerations.py
--rw-r--r--   0 korsch    (1000) korsch    (1000)      524 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/cvargparse/utils/logger_config.py
-drwxr-xr-x   0 korsch    (1000) korsch    (1000)        0 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/cvargparse.egg-info/
--rw-r--r--   0 korsch    (1000) korsch    (1000)      233 2024-03-07 12:24:50.000000 cvargparse-0.5.3.1/cvargparse.egg-info/PKG-INFO
--rw-r--r--   0 korsch    (1000) korsch    (1000)      606 2024-03-07 12:24:50.000000 cvargparse-0.5.3.1/cvargparse.egg-info/SOURCES.txt
--rw-r--r--   0 korsch    (1000) korsch    (1000)        1 2024-03-07 12:24:50.000000 cvargparse-0.5.3.1/cvargparse.egg-info/dependency_links.txt
--rw-r--r--   0 korsch    (1000) korsch    (1000)        1 2024-03-07 12:24:36.000000 cvargparse-0.5.3.1/cvargparse.egg-info/not-zip-safe
--rw-r--r--   0 korsch    (1000) korsch    (1000)        6 2024-03-07 12:24:50.000000 cvargparse-0.5.3.1/cvargparse.egg-info/requires.txt
--rw-r--r--   0 korsch    (1000) korsch    (1000)       11 2024-03-07 12:24:50.000000 cvargparse-0.5.3.1/cvargparse.egg-info/top_level.txt
--rw-r--r--   0 korsch    (1000) korsch    (1000)        6 2024-03-07 12:24:18.000000 cvargparse-0.5.3.1/requirements.txt
--rw-r--r--   0 korsch    (1000) korsch    (1000)       38 2024-03-07 12:24:50.344430 cvargparse-0.5.3.1/setup.cfg
--rw-r--r--   0 korsch    (1000) korsch    (1000)      999 2024-03-07 12:15:03.000000 cvargparse-0.5.3.1/setup.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2024-05-10 09:36:16.669000 cvargparse-0.5.4/
+-rw-r--r--   0 korsch   (10001) users    (10000)      148 2018-08-01 14:15:45.000000 cvargparse-0.5.4/.editorconfig
+-rw-r--r--   0 korsch   (10001) users    (10000)      728 2018-08-01 12:43:34.000000 cvargparse-0.5.4/.gitignore
+-rw-r--r--   0 korsch   (10001) users    (10000)      244 2019-11-06 08:29:47.000000 cvargparse-0.5.4/Makefile
+-rw-r--r--   0 korsch   (10001) users    (10000)      278 2024-05-10 09:36:16.669000 cvargparse-0.5.4/PKG-INFO
+-rw-r--r--   0 korsch   (10001) users    (10000)     3678 2024-03-07 12:19:55.000000 cvargparse-0.5.4/README.md
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2024-05-10 09:36:16.669000 cvargparse-0.5.4/cvargparse/
+-rw-r--r--   0 korsch   (10001) users    (10000)      950 2021-11-04 14:03:24.000000 cvargparse-0.5.4/cvargparse/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)       22 2024-05-10 09:36:11.000000 cvargparse-0.5.4/cvargparse/_version.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      877 2024-03-07 12:19:55.000000 cvargparse-0.5.4/cvargparse/argument.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1428 2021-11-04 09:30:20.000000 cvargparse-0.5.4/cvargparse/factory.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2024-05-10 09:36:16.669000 cvargparse-0.5.4/cvargparse/parser/
+-rw-r--r--   0 korsch   (10001) users    (10000)        0 2020-12-09 09:08:51.000000 cvargparse-0.5.4/cvargparse/parser/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     4325 2022-02-01 13:03:57.000000 cvargparse-0.5.4/cvargparse/parser/base.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      262 2021-11-04 09:36:24.000000 cvargparse-0.5.4/cvargparse/parser/gpu_parser.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      978 2020-12-09 09:30:43.000000 cvargparse-0.5.4/cvargparse/parser/mode_parser.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2024-05-10 09:36:16.669000 cvargparse-0.5.4/cvargparse/utils/
+-rw-r--r--   0 korsch   (10001) users    (10000)      151 2019-11-04 12:28:49.000000 cvargparse-0.5.4/cvargparse/utils/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2962 2024-05-10 08:58:36.000000 cvargparse-0.5.4/cvargparse/utils/dataclass.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      208 2018-09-24 07:42:39.000000 cvargparse-0.5.4/cvargparse/utils/decorators.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1497 2020-10-23 14:28:22.000000 cvargparse-0.5.4/cvargparse/utils/enumerations.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      524 2020-03-12 13:58:14.000000 cvargparse-0.5.4/cvargparse/utils/logger_config.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2024-05-10 09:36:16.669000 cvargparse-0.5.4/cvargparse.egg-info/
+-rw-r--r--   0 korsch   (10001) users    (10000)      278 2024-05-10 09:36:16.000000 cvargparse-0.5.4/cvargparse.egg-info/PKG-INFO
+-rw-r--r--   0 korsch   (10001) users    (10000)      657 2024-05-10 09:36:16.000000 cvargparse-0.5.4/cvargparse.egg-info/SOURCES.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)        1 2024-05-10 09:36:16.000000 cvargparse-0.5.4/cvargparse.egg-info/dependency_links.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)        1 2018-08-01 12:47:20.000000 cvargparse-0.5.4/cvargparse.egg-info/not-zip-safe
+-rw-r--r--   0 korsch   (10001) users    (10000)       12 2024-05-10 09:36:16.000000 cvargparse-0.5.4/cvargparse.egg-info/requires.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)       11 2024-05-10 09:36:16.000000 cvargparse-0.5.4/cvargparse.egg-info/top_level.txt
+-rwxr-xr-x   0 korsch   (10001) users    (10000)      251 2019-11-06 08:33:10.000000 cvargparse-0.5.4/deploy_latest.sh
+-rw-r--r--   0 korsch   (10001) users    (10000)       12 2023-09-28 07:09:42.000000 cvargparse-0.5.4/requirements.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)       38 2024-05-10 09:36:16.669000 cvargparse-0.5.4/setup.cfg
+-rw-r--r--   0 korsch   (10001) users    (10000)      985 2021-11-04 12:58:59.000000 cvargparse-0.5.4/setup.py
```

### Comparing `cvargparse-0.5.3.1/README.md` & `cvargparse-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/__init__.py` & `cvargparse-0.5.4/cvargparse/__init__.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/argument.py` & `cvargparse-0.5.4/cvargparse/argument.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/factory.py` & `cvargparse-0.5.4/cvargparse/factory.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/parser/base.py` & `cvargparse-0.5.4/cvargparse/parser/base.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/parser/mode_parser.py` & `cvargparse-0.5.4/cvargparse/parser/mode_parser.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/utils/dataclass.py` & `cvargparse-0.5.4/cvargparse/utils/dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 	return dataclass_args
 
 
 def cvdataclass(cls=None, *args, repr=False, **kwargs):
 
 	def _yaml_repr_(self) -> str:
 		cls_name = type(self).__name__
-		return yaml.dump({cls_name: self.__dict__}, sort_dicts=False)
+		return yaml.dump({cls_name: self.__dict__}, sort_keys=False)
 
 	def wrap(cls):
 		if not repr:
 			_set_attr(cls, "__repr__", _yaml_repr_)
 
 		return dataclass(cls, *args, repr=repr, **kwargs)
```

### Comparing `cvargparse-0.5.3.1/cvargparse/utils/enumerations.py` & `cvargparse-0.5.4/cvargparse/utils/enumerations.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/cvargparse/utils/logger_config.py` & `cvargparse-0.5.4/cvargparse/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `cvargparse-0.5.3.1/setup.py` & `cvargparse-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open(str(cwd / pkg_name / '_version.py')) as version_file:
 	exec(version_file.read())
 
 install_requires = [line.strip() for line in open("requirements.txt").readlines()]
 
 setup(
 	name=pkg_name,
-	version=__version__,  # noqa: F821
+	version=__version__,
 	description='simple argparse wrapper with some syntactic sugar',
 	author='Dimitri Korsch, Christoph Theiß',
 	author_email='korschdima@gmail.com, theisz.cm@gmail.com',
 	license='MIT License',
 	packages=find_packages(),
 	zip_safe=False,
 	setup_requires=[],
```

