# Comparing `tmp/elucidoc-2024.5.8.tar.gz` & `tmp/elucidoc-2024.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elucidoc-2024.5.8.tar", last modified: Thu May  9 01:07:47 2024, max compression
+gzip compressed data, was "elucidoc-2024.5.9.tar", last modified: Thu May  9 22:51:17 2024, max compression
```

## Comparing `elucidoc-2024.5.8.tar` & `elucidoc-2024.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.356150 elucidoc-2024.5.8/
--rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.8/LICENSE.txt
--rw-rw-rw-   0        0        0    10565 2024-05-09 01:07:47.354159 elucidoc-2024.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     7923 2024-05-09 01:03:05.000000 elucidoc-2024.5.8/README.md
--rw-rw-rw-   0        0        0      984 2024-05-09 01:05:03.000000 elucidoc-2024.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 01:07:47.357169 elucidoc-2024.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.332200 elucidoc-2024.5.8/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.340473 elucidoc-2024.5.8/src/elucidoc/
--rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.8/src/elucidoc/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.8/src/elucidoc/__main__.py
--rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.8/src/elucidoc/accessory.py
--rw-rw-rw-   0        0        0     7701 2024-05-08 12:53:41.000000 elucidoc-2024.5.8/src/elucidoc/eluciDoc.py
-drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.351152 elucidoc-2024.5.8/src/elucidoc.egg-info/
--rw-rw-rw-   0        0        0    10565 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.718785 elucidoc-2024.5.9/
+-rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    10677 2024-05-09 22:51:17.717786 elucidoc-2024.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8035 2024-05-09 10:58:07.000000 elucidoc-2024.5.9/README.md
+-rw-rw-rw-   0        0        0      984 2024-05-09 22:49:09.000000 elucidoc-2024.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 22:51:17.718785 elucidoc-2024.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.698182 elucidoc-2024.5.9/src/
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.704783 elucidoc-2024.5.9/src/elucidoc/
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.9/src/elucidoc/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.9/src/elucidoc/__main__.py
+-rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.9/src/elucidoc/accessory.py
+-rw-rw-rw-   0        0        0     7701 2024-05-08 12:53:41.000000 elucidoc-2024.5.9/src/elucidoc/eluciDoc.py
+drwxrwxrwx   0        0        0        0 2024-05-09 22:51:17.715787 elucidoc-2024.5.9/src/elucidoc.egg-info/
+-rw-rw-rw-   0        0        0    10677 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-09 22:51:17.000000 elucidoc-2024.5.9/src/elucidoc.egg-info/top_level.txt
```

### Comparing `elucidoc-2024.5.8/LICENSE.txt` & `elucidoc-2024.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.8/PKG-INFO` & `elucidoc-2024.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.8
+Version: 2024.5.9
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
@@ -109,22 +109,22 @@
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
 # Running the Script
-The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
-run by through a .bat file similar to:
+The project is run as a script.  It can be run with a .bat file calling the virtual environment and the executable
+file per the below example:
 ```commandline
 @"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
 
 @pause
 ```
-
+Additionally, the location of the ```elucidoc.py``` executable can be included in the Windows ```PATH``` environment variable.
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
 Textacy divides the party search term from both following words and punctuation including the possessive case, as shown below:
```

### Comparing `elucidoc-2024.5.8/README.md` & `elucidoc-2024.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
 # Running the Script
-The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
-run by through a .bat file similar to:
+The project is run as a script.  It can be run with a .bat file calling the virtual environment and the executable
+file per the below example:
 ```commandline
 @"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
 
 @pause
 ```
-
+Additionally, the location of the ```elucidoc.py``` executable can be included in the Windows ```PATH``` environment variable.
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
 Textacy divides the party search term from both following words and punctuation including the possessive case, as shown below:
```

### Comparing `elucidoc-2024.5.8/pyproject.toml` & `elucidoc-2024.5.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires      = ["setuptools >=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elucidoc"
-version = "2024.5.8"
+version = "2024.5.9"
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
 
+[project.scripts]
+elucidoc = "elucidoc.elucidoc:main_cli"
+
 [project.urls]
 "Source Code" = "https://github.com/jblake1965/eluciDoc"
 "License" = "https://github.com/jblake1965/eluciDoc/blob/developer/LICENSE.txt"
-
-[project.scripts]
-elucidoc = "elucidoc.__main__:main"
-
-
```

### Comparing `elucidoc-2024.5.8/src/elucidoc/accessory.py` & `elucidoc-2024.5.9/src/elucidoc/accessory.py`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.8/src/elucidoc/eluciDoc.py` & `elucidoc-2024.5.9/src/elucidoc/eluciDoc.py`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.8/src/elucidoc.egg-info/PKG-INFO` & `elucidoc-2024.5.9/src/elucidoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.8
+Version: 2024.5.9
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
@@ -109,22 +109,22 @@
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
 # Running the Script
-The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
-run by through a .bat file similar to:
+The project is run as a script.  It can be run with a .bat file calling the virtual environment and the executable
+file per the below example:
 ```commandline
 @"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
 
 @pause
 ```
-
+Additionally, the location of the ```elucidoc.py``` executable can be included in the Windows ```PATH``` environment variable.
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
 Textacy divides the party search term from both following words and punctuation including the possessive case, as shown below:
```

