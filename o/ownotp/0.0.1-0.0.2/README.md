# Comparing `tmp/ownotp-0.0.1.tar.gz` & `tmp/ownotp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownotp-0.0.1.tar", last modified: Fri May 10 12:12:02 2024, max compression
+gzip compressed data, was "ownotp-0.0.2.tar", last modified: Fri May 10 12:29:33 2024, max compression
```

## Comparing `ownotp-0.0.1.tar` & `ownotp-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:12:02.359928 ownotp-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 12:11:58.000000 ownotp-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 12:12:02.359928 ownotp-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 12:11:58.000000 ownotp-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:12:02.359928 ownotp-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-10 12:11:58.000000 ownotp-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:12:02.355929 ownotp-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:12:02.359928 ownotp-0.0.1/src/ownotp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 12:12:02.000000 ownotp-0.0.1/src/ownotp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 12:12:02.000000 ownotp-0.0.1/src/ownotp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:12:02.000000 ownotp-0.0.1/src/ownotp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:12:02.000000 ownotp-0.0.1/src/ownotp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:12:02.359928 ownotp-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:11:58.000000 ownotp-0.0.1/tests/test_otp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:29:33.203426 ownotp-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 12:29:25.000000 ownotp-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 12:29:33.203426 ownotp-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 12:29:25.000000 ownotp-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:29:33.199426 ownotp-0.0.2/ownotp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:29:25.000000 ownotp-0.0.2/ownotp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-10 12:29:25.000000 ownotp-0.0.2/ownotp/otp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:29:33.203426 ownotp-0.0.2/ownotp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 12:29:33.000000 ownotp-0.0.2/ownotp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 12:29:33.000000 ownotp-0.0.2/ownotp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:29:33.000000 ownotp-0.0.2/ownotp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 12:29:33.000000 ownotp-0.0.2/ownotp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:29:33.203426 ownotp-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-10 12:29:25.000000 ownotp-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:29:33.203426 ownotp-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:29:25.000000 ownotp-0.0.2/tests/test_otp.py
```

### Comparing `ownotp-0.0.1/LICENSE` & `ownotp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ownotp-0.0.1/setup.py` & `ownotp-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ownotp',
-    version='0.0.1',
+    version='0.0.2',
     author='karthiksenniyappan',
     author_email='karthiksenniyappan76@gmail.com',
     description="Generate a time-based OTP using SHA-256 hashing algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/karthiksenniyappan/ownotp",
-    packages=setuptools.find_packages(where='src'),
-    package_dir={'': 'src'},
+    packages=['ownotp'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

