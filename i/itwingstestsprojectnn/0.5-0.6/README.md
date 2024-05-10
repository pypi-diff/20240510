# Comparing `tmp/itwingstestsprojectnn-0.5.tar.gz` & `tmp/itwingstestsprojectnn-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwingstestsprojectnn-0.5.tar", last modified: Fri May 10 06:56:11 2024, max compression
+gzip compressed data, was "itwingstestsprojectnn-0.6.tar", last modified: Fri May 10 08:03:29 2024, max compression
```

## Comparing `itwingstestsprojectnn-0.5.tar` & `itwingstestsprojectnn-0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 06:56:11.692543 itwingstestsprojectnn-0.5/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.5/LICENSE
--rw-rw-rw-   0        0        0      393 2024-05-10 06:56:11.692543 itwingstestsprojectnn-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.5/README.md
--rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.5/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-05-10 06:56:11.696541 itwingstestsprojectnn-0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 06:56:11.640572 itwingstestsprojectnn-0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 06:56:11.690544 itwingstestsprojectnn-0.5/src/itwingstestsprojectnn.egg-info/
--rw-rw-rw-   0        0        0      393 2024-05-10 06:56:11.000000 itwingstestsprojectnn-0.5/src/itwingstestsprojectnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-05-10 06:56:11.000000 itwingstestsprojectnn-0.5/src/itwingstestsprojectnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 06:56:11.000000 itwingstestsprojectnn-0.5/src/itwingstestsprojectnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 06:56:11.000000 itwingstestsprojectnn-0.5/src/itwingstestsprojectnn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 06:56:11.683549 itwingstestsprojectnn-0.5/src/mymodule/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.5/src/mymodule/__init__.py
--rw-rw-rw-   0        0        0     5345 2024-05-10 06:52:18.000000 itwingstestsprojectnn-0.5/src/mymodule/main.py
--rw-rw-rw-   0        0        0     2016 2024-05-10 06:50:06.000000 itwingstestsprojectnn-0.5/src/mymodule/raw_data_to_csv.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:03:29.169661 itwingstestsprojectnn-0.6/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.6/LICENSE
+-rw-rw-rw-   0        0        0      393 2024-05-10 08:03:29.168661 itwingstestsprojectnn-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.6/README.md
+-rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-05-10 08:03:29.173658 itwingstestsprojectnn-0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 08:03:29.073717 itwingstestsprojectnn-0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 08:03:29.166662 itwingstestsprojectnn-0.6/src/itwingstestsprojectnn.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-10 08:03:28.000000 itwingstestsprojectnn-0.6/src/itwingstestsprojectnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-10 08:03:29.000000 itwingstestsprojectnn-0.6/src/itwingstestsprojectnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:03:28.000000 itwingstestsprojectnn-0.6/src/itwingstestsprojectnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 08:03:28.000000 itwingstestsprojectnn-0.6/src/itwingstestsprojectnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 08:03:29.159665 itwingstestsprojectnn-0.6/src/mymodule/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.6/src/mymodule/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-10 07:49:32.000000 itwingstestsprojectnn-0.6/src/mymodule/config.py
+-rw-rw-rw-   0        0        0     8897 2024-05-10 08:03:01.000000 itwingstestsprojectnn-0.6/src/mymodule/main.py
+-rw-rw-rw-   0        0        0     2016 2024-05-10 06:50:06.000000 itwingstestsprojectnn-0.6/src/mymodule/raw_data_to_csv.py
```

### Comparing `itwingstestsprojectnn-0.5/setup.cfg` & `itwingstestsprojectnn-0.6/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7477 696e 6773 7465 7374 7370   = itwingstestsp
 00000020: 726f 6a65 6374 6e6e 0d0a 7665 7273 696f  rojectnn..versio
-00000030: 6e20 3d20 302e 350d 0a61 7574 686f 7220  n = 0.5..author 
+00000030: 6e20 3d20 302e 360d 0a61 7574 686f 7220  n = 0.6..author 
 00000040: 3d20 4d61 7961 6e6b 0d0a 6175 7468 6f72  = Mayank..author
 00000050: 5f65 6d61 696c 203d 206d 6179 616e 6b74  _email = mayankt
 00000060: 696d 6261 6469 6140 676d 6169 6c2e 636f  imbadia@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2073 6d61 6c6c 2065 7861 6d70 6c65   A small example
 00000090: 2070 6163 6b61 6765 0d0a 6c6f 6e67 5f64   package..long_d
 000000a0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `itwingstestsprojectnn-0.5/src/mymodule/raw_data_to_csv.py` & `itwingstestsprojectnn-0.6/src/mymodule/raw_data_to_csv.py`

 * *Files identical despite different names*

