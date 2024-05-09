# Comparing `tmp/elucidoc-2024.5.5.tar.gz` & `tmp/elucidoc-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elucidoc-2024.5.5.tar", last modified: Sun May  5 13:49:49 2024, max compression
+gzip compressed data, was "elucidoc-2024.5.8.tar", last modified: Thu May  9 01:07:47 2024, max compression
```

## Comparing `elucidoc-2024.5.5.tar` & `elucidoc-2024.5.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 13:49:49.698497 elucidoc-2024.5.5/
--rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0    10269 2024-05-05 13:49:49.697512 elucidoc-2024.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     7627 2024-04-29 22:57:10.000000 elucidoc-2024.5.5/README.md
--rw-rw-rw-   0        0        0      926 2024-05-05 13:49:30.000000 elucidoc-2024.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 13:49:49.699469 elucidoc-2024.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 13:49:49.680473 elucidoc-2024.5.5/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:49:49.686470 elucidoc-2024.5.5/src/elucidoc/
--rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.5/src/elucidoc/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.5/src/elucidoc/__main__.py
--rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.5/src/elucidoc/accessory.py
--rw-rw-rw-   0        0        0     7659 2024-04-13 11:19:13.000000 elucidoc-2024.5.5/src/elucidoc/eluciDoc.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:49:49.695467 elucidoc-2024.5.5/src/elucidoc.egg-info/
--rw-rw-rw-   0        0        0    10269 2024-05-05 13:49:49.000000 elucidoc-2024.5.5/src/elucidoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-05-05 13:49:49.000000 elucidoc-2024.5.5/src/elucidoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 13:49:49.000000 elucidoc-2024.5.5/src/elucidoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-05 13:49:49.000000 elucidoc-2024.5.5/src/elucidoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-05 13:49:49.000000 elucidoc-2024.5.5/src/elucidoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.356150 elucidoc-2024.5.8/
+-rw-rw-rw-   0        0        0     1558 2023-12-12 02:24:07.000000 elucidoc-2024.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    10565 2024-05-09 01:07:47.354159 elucidoc-2024.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7923 2024-05-09 01:03:05.000000 elucidoc-2024.5.8/README.md
+-rw-rw-rw-   0        0        0      984 2024-05-09 01:05:03.000000 elucidoc-2024.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 01:07:47.357169 elucidoc-2024.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.332200 elucidoc-2024.5.8/src/
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:23:02.000000 elucidoc-2024.5.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.340473 elucidoc-2024.5.8/src/elucidoc/
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:41:07.000000 elucidoc-2024.5.8/src/elucidoc/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:26:16.000000 elucidoc-2024.5.8/src/elucidoc/__main__.py
+-rw-rw-rw-   0        0        0      665 2024-04-06 13:56:35.000000 elucidoc-2024.5.8/src/elucidoc/accessory.py
+-rw-rw-rw-   0        0        0     7701 2024-05-08 12:53:41.000000 elucidoc-2024.5.8/src/elucidoc/eluciDoc.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:07:47.351152 elucidoc-2024.5.8/src/elucidoc.egg-info/
+-rw-rw-rw-   0        0        0    10565 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-09 01:07:47.000000 elucidoc-2024.5.8/src/elucidoc.egg-info/top_level.txt
```

### Comparing `elucidoc-2024.5.5/LICENSE.txt` & `elucidoc-2024.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.5/PKG-INFO` & `elucidoc-2024.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.5
+Version: 2024.5.8
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
@@ -108,14 +108,22 @@
 
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
+# Running the Script
+The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
+run by through a .bat file similar to:
+```commandline
+@"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
+
+@pause
+```
 
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
```

### Comparing `elucidoc-2024.5.5/README.md` & `elucidoc-2024.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,22 @@
 
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
+# Running the Script
+The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
+run by through a .bat file similar to:
+```commandline
+@"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
+
+@pause
+```
 
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
```

### Comparing `elucidoc-2024.5.5/pyproject.toml` & `elucidoc-2024.5.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elucidoc"
-version = "2024.5.5"
+version = "2024.5.8"
 license = {file = "LICENSE.txt"}
 description = "Screens legal and other texts for sentences and clauses containing user defined search phrases"
 readme = "README.md"
 authors = [{name = 'John Blake'}, {email = "elucidoc535@gmail.com"}]
 
 classifiers = [
     "Programming Language :: Python",
@@ -18,8 +18,11 @@
 keywords = ["legal", "text", "analysis"]
 dependencies = ["docx2python==2.10.1", "openpyxl==3.1.2", "pandas==2.2.2", "pdfminer.six==20231228", "python-docx==1.1.2", "rich==13.7.1", "spacy==3.7.4", "textacy==0.13.0"]
 
 [project.urls]
 "Source Code" = "https://github.com/jblake1965/eluciDoc"
 "License" = "https://github.com/jblake1965/eluciDoc/blob/developer/LICENSE.txt"
 
+[project.scripts]
+elucidoc = "elucidoc.__main__:main"
+
```

### Comparing `elucidoc-2024.5.5/src/elucidoc/accessory.py` & `elucidoc-2024.5.8/src/elucidoc/accessory.py`

 * *Files identical despite different names*

### Comparing `elucidoc-2024.5.5/src/elucidoc/eluciDoc.py` & `elucidoc-2024.5.8/src/elucidoc/eluciDoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                 text = extract_text(target_File)
                 text = text_cleanup(text)
                 text = pdf_cleanup(text)
             if file_extension == '.txt':
                 target = open(target_File, 'r', encoding='utf8')
                 text = target.read()
                 text = text_cleanup(text)
+                text = pdf_cleanup(text)
         break
 
 while True:
     print("")
     case_sensitive = console.input('[bold green italic]IS THIS SEARCH CASE SENSITIVE?: YES or NO [/]')
     print("")
     case_sensitive = case_sensitive.lower()
```

### Comparing `elucidoc-2024.5.5/src/elucidoc.egg-info/PKG-INFO` & `elucidoc-2024.5.8/src/elucidoc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elucidoc
-Version: 2024.5.5
+Version: 2024.5.8
 Summary: Screens legal and other texts for sentences and clauses containing user defined search phrases
 Author: John Blake
 Author-email: elucidoc535@gmail.com
 License: Copyright 2023 John R. Blake, Jr.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
@@ -108,14 +108,22 @@
 
 The pipeline can be installed as follows:
 ```
 python -m spacy download en_core_web_lg
 ```
 You must also be sure to verify the directory for the Office install is the same as noted above.  If not, the code must be 
 changed to the directory where the Excel and Word apps are located.
+# Running the Script
+The project is run as a script by typing the command "elucidoc" in the virtual environment.  Alternatively, it can be
+run by through a .bat file similar to:
+```commandline
+@"C:\Users\..\venv\Scripts\python.exe" "C:\Users\..\venv\lib\elucidoc\eluciDoc.py"
+
+@pause
+```
 
 # Case Sensitive Searches
 General convention in legal texts is to capitalize defined terms.  For that reason, the user may want to make the search
 case-sensitive to target the appropriate instances of the term.  For searches where the specific use of the subject term
 is not important but broader capture is, the case-sensitive feature can be turned off.  Once a selection is made, it applies
 for all subsequent searches until the script is restarted.
 # Possessive Case and Other Punctuation
```

