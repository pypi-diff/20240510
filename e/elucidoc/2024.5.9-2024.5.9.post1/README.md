# Comparing `tmp/elucidoc-2024.5.9.tar.gz` & `tmp/elucidoc-2024.5.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elucidoc-2024.5.9.tar", last modified: Thu May  9 22:51:17 2024, max compression
+gzip compressed data, was "elucidoc-2024.5.9.post1.tar", last modified: Fri May 10 00:54:30 2024, max compression
```

## Comparing `elucidoc-2024.5.9.tar` & `elucidoc-2024.5.9.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.718785 elucidoc-2024.5.9/
--rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.9/LICENSE.txt
--rw-rw-rw-   0        0        0    10677 2024-05-09 22:51:17.717786 elucidoc-2024.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     8035 2024-05-09 10:58:07.000000 elucidoc-2024.5.9/README.md
--rw-rw-rw-   0        0        0      984 2024-05-09 22:49:09.000000 elucidoc-2024.5.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 22:51:17.718785 elucidoc-2024.5.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.698182 elucidoc-2024.5.9/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.704783 elucidoc-2024.5.9/src/elucidoc/
--rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.9/src/elucidoc/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.9/src/elucidoc/__main__.py
--rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.9/src/elucidoc/accessory.py
--rw-rw-rw-   0        0        0     7701 2024-05-08 12:53:41.000000 elucidoc-2024.5.9/src/elucidoc/eluciDoc.py
-drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.715787 elucidoc-2024.5.9/src/elucidoc.egg-info/
--rw-rw-rw-   0        0        0    10677 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 00:54:30.737485 elucidoc-2024.5.9.post1/
+-rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.9.post1/LICENSE.txt
+-rw-rw-rw-   0        0        0    10683 2024-05-10 00:54:30.736481 elucidoc-2024.5.9.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     8035 2024-05-09 10:58:07.000000 elucidoc-2024.5.9.post1/README.md
+-rw-rw-rw-   0        0        0      977 2024-05-10 00:53:56.000000 elucidoc-2024.5.9.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:54:30.737485 elucidoc-2024.5.9.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 00:54:30.721138 elucidoc-2024.5.9.post1/src/
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.9.post1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:54:30.726146 elucidoc-2024.5.9.post1/src/elucidoc/
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.9.post1/src/elucidoc/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.9.post1/src/elucidoc/__main__.py
+-rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.9.post1/src/elucidoc/accessory.py
+-rw-rw-rw-   0        0        0     7701 2024-05-08 12:53:41.000000 elucidoc-2024.5.9.post1/src/elucidoc/eluciDoc.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:54:30.735480 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/
+-rw-rw-rw-   0        0        0    10683 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 00:54:30.000000 elucidoc-2024.5.9.post1/src/elucidoc.egg-info/top_level.txt
```

### Comparing `elucidoc-2024.5.9/LICENSE.txt` & `elucidoc-2024.5.9.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.9/PKG-INFO` & `elucidoc-2024.5.9.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.9
+Version: 2024.5.9.post1
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
```

### Comparing `elucidoc-2024.5.9/README.md` & `elucidoc-2024.5.9.post1/README.md`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.9/pyproject.toml` & `elucidoc-2024.5.9.post1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires      = ["setuptools >=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elucidoc"
-version = "2024.5.9"
+version = "2024.5.9-1"
 license = {file = "LICENSE.txt"}
 description = "Screens legal and other texts for sentences and clauses containing user defined search phrases"
 readme = "README.md"
 authors = [{name = 'John Blake'}, {email = "elucidoc535@gmail.com"}]
 
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License"
 ]
 keywords = ["legal", "text", "analysis"]
 dependencies = ["docx2python==2.10.1", "openpyxl==3.1.2", "pandas==2.2.2", "pdfminer.six==20231228", "python-docx==1.1.2", "rich==13.7.1", "spacy==3.7.4", "textacy==0.13.0"]
 
 [project.scripts]
-elucidoc = "elucidoc.elucidoc:main_cli"
+elucidoc = "elucidoc:main_cli"
 
 [project.urls]
 "Source Code" = "https://github.com/jblake1965/eluciDoc"
 "License" = "https://github.com/jblake1965/eluciDoc/blob/developer/LICENSE.txt"
```

### Comparing `elucidoc-2024.5.9/src/elucidoc/accessory.py` & `elucidoc-2024.5.9.post1/src/elucidoc/accessory.py`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.9/src/elucidoc/eluciDoc.py` & `elucidoc-2024.5.9.post1/src/elucidoc/eluciDoc.py`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.9/src/elucidoc.egg-info/PKG-INFO` & `elucidoc-2024.5.9.post1/src/elucidoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.9
+Version: 2024.5.9.post1
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
```

