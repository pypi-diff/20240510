# Comparing `tmp/stsci.image-2.3.5.tar.gz` & `tmp/stsci_image-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpdob_qdse/tmp_pkthkc2/stsci.image-2.3.5.tar", last modified: Mon Aug 30 18:51:08 2021, max compression
+gzip compressed data, was "stsci_image-2.3.7.tar", last modified: Fri May 10 13:29:24 2024, max compression
```

## Comparing `stsci.image-2.3.5.tar` & `stsci_image-2.3.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/
--rwxr-xr-x   0 root         (0) root         (0)     1144 2021-08-30 18:50:43.000000 stsci.image-2.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/src/
--rw-r--r--   0 root         (0) root         (0)     9490 2021-08-30 18:50:43.000000 stsci.image-2.3.5/src/_combinemodule.c
--rw-r--r--   0 root         (0) root         (0)      612 2021-08-30 18:51:08.000000 stsci.image-2.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2021-08-30 18:50:43.000000 stsci.image-2.3.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       77 2021-08-30 18:50:43.000000 stsci.image-2.3.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      184 2021-08-30 18:50:43.000000 stsci.image-2.3.5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci/
--rw-r--r--   0 root         (0) root         (0)      478 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci/image/
--rw-r--r--   0 root         (0) root         (0)    16306 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/numcombine.py
--rw-r--r--   0 root         (0) root         (0)      257 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2320 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/_image.py
--rw-r--r--   0 root         (0) root         (0)    13472 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/combine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci/image/test/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2418 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/test/test_average.py
--rw-r--r--   0 root         (0) root         (0)     2390 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/test/test_median.py
--rw-r--r--   0 root         (0) root         (0)     2400 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/test/test_minimum.py
--rw-r--r--   0 root         (0) root         (0)     2812 2021-08-30 18:50:43.000000 stsci.image-2.3.5/stsci/image/test/test_threshold.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/docs/
--rw-r--r--   0 root         (0) root         (0)     3138 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/docs/source/
--rw-r--r--   0 root         (0) root         (0)      525 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      298 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/source/numcombine.rst
--rw-r--r--   0 root         (0) root         (0)     6520 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)      362 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/source/image.rst
--rw-r--r--   0 root         (0) root         (0)     3083 2021-08-30 18:50:43.000000 stsci.image-2.3.5/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      855 2021-08-30 18:50:43.000000 stsci.image-2.3.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 root         (0) root         (0)     1016 2021-08-30 18:50:43.000000 stsci.image-2.3.5/.github/workflows/ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       33 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      612 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      698 2021-08-30 18:51:08.000000 stsci.image-2.3.5/stsci.image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-30 18:51:08.000000 stsci.image-2.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 13:29:11.000000 stsci_image-2.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 13:29:24.115718 stsci_image-2.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/numcombine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-10 13:29:11.000000 stsci_image-2.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:29:24.115718 stsci_image-2.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      310 2024-05-10 13:29:11.000000 stsci_image-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-10 13:29:11.000000 stsci_image-2.3.7/src/_combinemodule.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/stsci/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/stsci/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/numcombine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/stsci/image/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/stsci.image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:29:23.000000 stsci_image-2.3.7/stsci.image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stsci.image-2.3.5/setup.py` & `stsci_image-2.3.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,56 @@
-from setuptools import setup, find_packages, Extension
-from numpy import get_include as np_include
+[project]
+name = "stsci.image"
+description = "Image array manipulation functions"
+readme = "README.md"
+requires-python = ">=3.9"
+license = { file = "LICENSE" }
+authors = [{ name = "STScI", email = "help@stsci.edu" }]
+classifiers = [
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Scientific/Engineering :: Astronomy",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dependencies = [
+    "numpy",
+    "scipy",
+]
+dynamic = ['version']
 
-setup(
-    name='stsci.image',
-    author='STScI',
-    author_email='help@stsci.edu',
-    description='Image array manipulation functions',
-    url='https://github.com/spacetelescope/stsci.image',
-    classifiers=[
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Topic :: Scientific/Engineering :: Astronomy',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-    install_requires=[
-        'numpy>=1.14',
-        'scipy',
-    ],
-    packages=find_packages(),
-    package_data={
-        '': ['LICENSE.txt'],
-    },
-    ext_modules=[
-        Extension('stsci.image._combine',
-                  ['src/_combinemodule.c'],
-                  include_dirs=[np_include()],
-                  define_macros=[('NUMPY', '1')]),
-    ],
-    use_scm_version=True,
-    setup_requires=['setuptools_scm'],
-    extras_require={
-        "test": [
-            "pytest"
-        ]
-    }
-)
+[project.optional-dependencies]
+test = [
+    'pytest',
+]
+docs = [
+    'numpydoc',
+    'sphinx',
+    'sphinx-automodapi',
+    'sphinx-rtd-theme',
+    'stsci-rtd-theme',
+    'tomli; python_version <"3.11"',
+]
+
+[project.urls]
+'repository' = 'https://github.com/spacetelescope/stsci.image'
+
+[build-system]
+requires = [
+    "setuptools >=61.2",
+    "setuptools_scm[toml] >=6.2",
+    "wheel",
+    "oldest-supported-numpy",
+]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+zip-safe = false
+
+[tool.setuptools.packages.find]
+include = ['stsci']
+
+[tool.setuptools.package-data]
+"*" = ["LICENSE.txt"]
+
+[tool.setuptools_scm]
```

### Comparing `stsci.image-2.3.5/src/_combinemodule.c` & `stsci_image-2.3.7/src/_combinemodule.c`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/LICENSE.txt` & `stsci_image-2.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/stsci/image/numcombine.py` & `stsci_image-2.3.7/stsci/image/numcombine.py`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/stsci/image/_image.py` & `stsci_image-2.3.7/stsci/image/_image.py`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/stsci/image/combine.py` & `stsci_image-2.3.7/stsci/image/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
            [ 8, 12]])
     >>> median(arrays, nlow=1)
     array([[ 0,  8],
            [16, 24]])
     >>> median(arrays, outtype=np.float32)
     array([[ 0.,  6.],
            [12., 18.]], dtype=float32)
-    >>> bm = np.zeros((4,2,2), dtype=np.bool8)
+    >>> bm = np.zeros((4,2,2), dtype=bool)
     >>> bm[2,...] = 1
     >>> median(arrays, badmasks=bm)
     array([[ 0,  8],
            [16, 24]])
     >>> median(arrays, badmasks=threshhold(arrays, high=25))
     array([[ 0,  6],
            [ 8, 12]])
@@ -116,15 +116,15 @@
            [ 8, 12]])
     >>> median(arrays, nlow=1)
     array([[ 0,  8],
            [16, 24]])
     >>> median(arrays, outtype=np.float32)
     array([[ 0.,  6.],
            [12., 18.]], dtype=float32)
-    >>> bm = np.zeros((4,2,2), dtype=np.bool8)
+    >>> bm = np.zeros((4,2,2), dtype=bool)
     >>> bm[2,...] = 1
     >>> median(arrays, badmasks=bm)
     array([[ 0,  8],
            [16, 24]])
     >>> median(arrays, badmasks=threshhold(arrays, high=25))
     array([[ 0,  6],
            [ 8, 12]])
@@ -169,15 +169,15 @@
            [ 9, 14]])
     >>> average(arrays, nlow=1)
     array([[ 0,  9],
            [18, 28]])
     >>> average(arrays, outtype=np.float32)
     array([[ 0. ,  7.5],
            [15. , 22.5]], dtype=float32)
-    >>> bm = np.zeros((4,2,2), dtype=np.bool8)
+    >>> bm = np.zeros((4,2,2), dtype=bool)
     >>> bm[2,...] = 1
     >>> average(arrays, badmasks=bm)
     array([[ 0,  9],
            [18, 28]])
     >>> average(arrays, badmasks=threshhold(arrays, high=25))
     array([[ 0,  7],
            [ 9, 14]])
@@ -221,15 +221,15 @@
            [ 9, 14]])
     >>> average(arrays, nlow=1)
     array([[ 0,  9],
            [18, 28]])
     >>> average(arrays, outtype=np.float32)
     array([[ 0. ,  7.5],
            [15. , 22.5]], dtype=float32)
-    >>> bm = np.zeros((4,2,2), dtype=np.bool8)
+    >>> bm = np.zeros((4,2,2), dtype=bool)
     >>> bm[2,...] = 1
     >>> average(arrays, badmasks=bm)
     array([[ 0,  9],
            [18, 28]])
     >>> average(arrays, badmasks=threshhold(arrays, high=25))
     array([[ 0,  7],
            [ 9, 14]])
@@ -275,15 +275,15 @@
            [4, 6]])
     >>> minimum(arrays, nlow=1)
     array([[ 0,  4],
            [ 8, 12]])
     >>> minimum(arrays, outtype=np.float32)
     array([[0., 2.],
            [4., 6.]], dtype=float32)
-    >>> bm = np.zeros((4,2,2), dtype=np.bool8)
+    >>> bm = np.zeros((4,2,2), dtype=bool)
     >>> bm[2,...] = 1
     >>> minimum(arrays, badmasks=bm)
     array([[ 0,  4],
            [ 8, 12]])
     >>> minimum(arrays, badmasks=threshhold(arrays, low=10))
     array([[ 0, 16],
            [16, 12]])
@@ -383,9 +383,9 @@
     median(arrays)
     print("maskless:", time.clock()-t0)
 
     a = np.arange(10**6)
     a = a.reshape((1000, 1000))
     arrays = [a*2, a*64, a*16, a*8]
     t0 = time.clock()
-    median(arrays, badmasks=np.zeros((1000,1000), dtype=np.bool8))
+    median(arrays, badmasks=np.zeros((1000,1000), dtype=bool))
     print("masked:", time.clock()-t0)
```

### Comparing `stsci.image-2.3.5/stsci/image/test/test_average.py` & `stsci_image-2.3.7/stsci/image/test/test_average.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,22 +60,21 @@
     result = combine.average(arrays, outtype=np.float32)
     expected = np.array([[  0. ,   7.5],
                          [ 15. ,  22.5]], dtype=np.float32)
     assert (result == expected).all()
 
 
 def test_average5(arrays):
-    bm = np.zeros((4,2,2), dtype=np.bool8)
+    bm = np.zeros((4,2,2), dtype=bool)
     bm[2,...] = 1
     result = combine.average(arrays, badmasks=bm)
     expected = np.array([[ 0,  9],
                          [18, 28]])
     assert (result == expected).all()
 
 
 def test_average6(arrays):
     result = combine.average(arrays,
                              badmasks=combine.threshhold(arrays, high=25))
     expected = np.array([[ 0,  7],
                          [ 9, 14]])
     assert (result == expected).all()
-
```

### Comparing `stsci.image-2.3.5/stsci/image/test/test_median.py` & `stsci_image-2.3.7/stsci/image/test/test_median.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     result = combine.median(arrays, outtype=np.float32)
     expected = np.array([[  0.,   6.],
                          [ 12.,  18.]], dtype=np.float32)
     assert (result == expected).all()
 
 
 def test_median5(arrays):
-    bm = np.zeros((4,2,2), dtype=np.bool8)
+    bm = np.zeros((4,2,2), dtype=bool)
     bm[2,...] = 1
     result = combine.median(arrays, badmasks=bm)
     expected = np.array([[ 0,  8],
                          [16, 24]])
     assert (result == expected).all()
```

### Comparing `stsci.image-2.3.5/stsci/image/test/test_minimum.py` & `stsci_image-2.3.7/stsci/image/test/test_minimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     result = combine.minimum(arrays, outtype=np.float32)
     expected = np.array([[ 0.,  2.],
                          [ 4.,  6.]], dtype=np.float32)
     assert (result == expected).all()
 
 
 def test_minimum5(arrays):
-    bm = np.zeros((4,2,2), dtype=np.bool8)
+    bm = np.zeros((4,2,2), dtype=bool)
     bm[2,...] = 1
     result = combine.minimum(arrays, badmasks=bm)
     expected = np.array([[ 0,  4],
                          [ 8, 12]])
     assert (result == expected).all()
```

### Comparing `stsci.image-2.3.5/stsci/image/test/test_threshold.py` & `stsci_image-2.3.7/stsci/image/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/docs/Makefile` & `stsci_image-2.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/docs/source/index.rst` & `stsci_image-2.3.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/docs/source/conf.py` & `stsci_image-2.3.7/docs/source/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,195 +6,202 @@
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
+from datetime import datetime
+from pathlib import Path
 
-import sys, os
+if sys.version_info < (3, 11):
+     import tomli as tomllib
+ else:
+     import tomllib
 from stsci.sphinxext.conf import *
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
+# sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
+with open(Path(__file__).parent.parent.parent / "pyproject.toml", "rb") as metadata_file:
+    metadata = tomli.load(metadata_file)['project']
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions += ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
                'sphinx.ext.intersphinx', 'sphinx.ext.pngmath']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
-#source_encoding = 'utf-8'
+# source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'image'
-copyright = u'2012, STScI'
+project = metadata['name']
+author = f'{metadata["authors"][0]["name"]} <{metadata["authors"][0]["email"]}>'
+copyright = f'{datetime.today().year}, {author}'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '2.0'
 # The full version, including alpha/beta/rc tags.
 release = '2.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of documents that shouldn't be included in the build.
-#unused_docs = []
+# unused_docs = []
 
 # List of directories, relative to source directory, that shouldn't be searched
 # for source files.
 exclude_trees = []
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
-#html_theme = 'default'
+# html_theme = 'default'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_use_modindex = True
+# html_use_modindex = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # If nonempty, this is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = ''
+# html_file_suffix = ''
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'imagedoc'
 
-
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
+# latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
+# latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'image.tex', u'Image Documentation',
-   u'STScI', 'manual'),
+    ('index', 'image.tex', u'Image Documentation',
+     u'STScI', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
+# latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_use_modindex = True
+# latex_use_modindex = True
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {'http://docs.python.org/': None}
```

### Comparing `stsci.image-2.3.5/docs/make.bat` & `stsci_image-2.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stsci.image-2.3.5/.github/workflows/ci.yml` & `stsci_image-2.3.7/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
   ci:
     name: Python ${{ matrix.python-version }}, numpy${{ matrix.numpy-version }}
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
-          - python-version: 3.7
-            numpy-version: "~=1.14.0"
-        python-version: [3.7, 3.8, 3.9]
-        numpy-version: ["~=1.17.0", "~=1.19.0", ""]
+          - python-version: "3.12"
+            numpy-version: "~=1.26.0"
+        python-version: ["3.9", "3.10", "3.11"]
+        numpy-version: ["~=1.23.0", "~=1.26.0", ""]
 
     steps:
       - name: Checkout code
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
```

### Comparing `stsci.image-2.3.5/stsci.image.egg-info/SOURCES.txt` & `stsci_image-2.3.7/stsci.image.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 .gitignore
 LICENSE.txt
 pyproject.toml
 setup.py
+.github/workflows/build.yml
 .github/workflows/ci.yml
-.github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/image.rst
 docs/source/index.rst
 docs/source/numcombine.rst
 src/_combinemodule.c
 stsci/__init__.py
 stsci.image.egg-info/PKG-INFO
 stsci.image.egg-info/SOURCES.txt
 stsci.image.egg-info/dependency_links.txt
+stsci.image.egg-info/not-zip-safe
 stsci.image.egg-info/requires.txt
 stsci.image.egg-info/top_level.txt
 stsci/image/__init__.py
 stsci/image/_image.py
 stsci/image/combine.py
 stsci/image/numcombine.py
 stsci/image/test/__init__.py
```

