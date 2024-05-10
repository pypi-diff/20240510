# Comparing `tmp/txt-from-pdf-1.1.0.tar.gz` & `tmp/txt-from-pdf-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt-from-pdf-1.1.0.tar", last modified: Fri May  3 15:39:40 2024, max compression
+gzip compressed data, was "txt-from-pdf-1.1.1.tar", last modified: Fri May 10 11:39:04 2024, max compression
```

## Comparing `txt-from-pdf-1.1.0.tar` & `txt-from-pdf-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.651329 txt-from-pdf-1.1.0/
--rw-r--r--   0 asafaya    (501) staff       (20)    11357 2024-04-18 13:31:13.000000 txt-from-pdf-1.1.0/LICENSE
--rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-03 15:39:40.651221 txt-from-pdf-1.1.0/PKG-INFO
--rw-r--r--   0 asafaya    (501) staff       (20)     1592 2024-05-03 15:38:37.000000 txt-from-pdf-1.1.0/README.md
--rw-r--r--   0 asafaya    (501) staff       (20)      672 2024-04-18 13:38:51.000000 txt-from-pdf-1.1.0/pyproject.toml
--rw-r--r--   0 asafaya    (501) staff       (20)       38 2024-05-03 15:39:40.651373 txt-from-pdf-1.1.0/setup.cfg
--rw-r--r--   0 asafaya    (501) staff       (20)     2301 2024-05-03 15:36:47.000000 txt-from-pdf-1.1.0/setup.py
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.649738 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/
--rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/PKG-INFO
--rw-r--r--   0 asafaya    (501) staff       (20)      394 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 asafaya    (501) staff       (20)        1 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       62 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/entry_points.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       86 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/requires.txt
--rw-r--r--   0 asafaya    (501) staff       (20)       11 2024-05-03 15:39:40.000000 txt-from-pdf-1.1.0/txt_from_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-03 15:39:40.650937 txt-from-pdf-1.1.0/txtfrompdf/
--rw-r--r--   0 asafaya    (501) staff       (20)      255 2024-05-03 15:36:29.000000 txt-from-pdf-1.1.0/txtfrompdf/__init__.py
--rw-r--r--   0 asafaya    (501) staff       (20)     2361 2024-04-18 16:20:19.000000 txt-from-pdf-1.1.0/txtfrompdf/__main__.py
--rw-r--r--   0 asafaya    (501) staff       (20)     4903 2024-04-30 20:35:51.000000 txt-from-pdf-1.1.0/txtfrompdf/extract.py
--rw-r--r--   0 asafaya    (501) staff       (20)     6575 2024-04-18 13:38:56.000000 txt-from-pdf-1.1.0/txtfrompdf/filter.py
--rw-r--r--   0 asafaya    (501) staff       (20)     3296 2024-04-30 20:26:33.000000 txt-from-pdf-1.1.0/txtfrompdf/fix_unicode.py
--rw-r--r--   0 asafaya    (501) staff       (20)      511 2024-04-18 13:14:27.000000 txt-from-pdf-1.1.0/txtfrompdf/utils.py
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-10 11:39:04.713395 txt-from-pdf-1.1.1/
+-rw-r--r--   0 asafaya    (501) staff       (20)    11357 2024-04-18 13:31:13.000000 txt-from-pdf-1.1.1/LICENSE
+-rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-10 11:39:04.713287 txt-from-pdf-1.1.1/PKG-INFO
+-rw-r--r--   0 asafaya    (501) staff       (20)     1592 2024-05-03 15:38:37.000000 txt-from-pdf-1.1.1/README.md
+-rw-r--r--   0 asafaya    (501) staff       (20)      672 2024-04-18 13:38:51.000000 txt-from-pdf-1.1.1/pyproject.toml
+-rw-r--r--   0 asafaya    (501) staff       (20)       38 2024-05-10 11:39:04.713434 txt-from-pdf-1.1.1/setup.cfg
+-rw-r--r--   0 asafaya    (501) staff       (20)     2301 2024-05-10 11:38:05.000000 txt-from-pdf-1.1.1/setup.py
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-10 11:39:04.711923 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/
+-rw-r--r--   0 asafaya    (501) staff       (20)     2428 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 asafaya    (501) staff       (20)      394 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)        1 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       62 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/entry_points.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       86 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/requires.txt
+-rw-r--r--   0 asafaya    (501) staff       (20)       11 2024-05-10 11:39:04.000000 txt-from-pdf-1.1.1/txt_from_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 asafaya    (501) staff       (20)        0 2024-05-10 11:39:04.713002 txt-from-pdf-1.1.1/txtfrompdf/
+-rw-r--r--   0 asafaya    (501) staff       (20)      255 2024-05-10 11:37:55.000000 txt-from-pdf-1.1.1/txtfrompdf/__init__.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     2361 2024-04-18 16:20:19.000000 txt-from-pdf-1.1.1/txtfrompdf/__main__.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     5600 2024-05-10 11:37:23.000000 txt-from-pdf-1.1.1/txtfrompdf/extract.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     6575 2024-04-18 13:38:56.000000 txt-from-pdf-1.1.1/txtfrompdf/filter.py
+-rw-r--r--   0 asafaya    (501) staff       (20)     3296 2024-04-30 20:26:33.000000 txt-from-pdf-1.1.1/txtfrompdf/fix_unicode.py
+-rw-r--r--   0 asafaya    (501) staff       (20)      511 2024-04-18 13:14:27.000000 txt-from-pdf-1.1.1/txtfrompdf/utils.py
```

### Comparing `txt-from-pdf-1.1.0/LICENSE` & `txt-from-pdf-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.1.0/PKG-INFO` & `txt-from-pdf-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt-from-pdf
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extract clean text from PDFs.
 Home-page: https://github.com/alisafaya/txt-from-pdf
 Author: Ali Safaya
 Author-email: alisafaya@gmail.com
 License: Apache
 Keywords: pdf text extraction
 Classifier: Intended Audience :: Developers
```

### Comparing `txt-from-pdf-1.1.0/README.md` & `txt-from-pdf-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.1.0/pyproject.toml` & `txt-from-pdf-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.1.0/setup.py` & `txt-from-pdf-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 extras = {}
 extras["dev"] = ["black ~= 23.0", "ruff>=0.2"]
 
 setup(
     name="txt-from-pdf",
-    version="1.1.0",
+    version="1.1.1",
     description="Extract clean text from PDFs.",
     license_files=["LICENSE"],
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="pdf text extraction",
     license="Apache",
     author="Ali Safaya",
```

### Comparing `txt-from-pdf-1.1.0/txt_from_pdf.egg-info/PKG-INFO` & `txt-from-pdf-1.1.1/txt_from_pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt-from-pdf
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extract clean text from PDFs.
 Home-page: https://github.com/alisafaya/txt-from-pdf
 Author: Ali Safaya
 Author-email: alisafaya@gmail.com
 License: Apache
 Keywords: pdf text extraction
 Classifier: Intended Audience :: Developers
```

### Comparing `txt-from-pdf-1.1.0/txtfrompdf/__main__.py` & `txt-from-pdf-1.1.1/txtfrompdf/__main__.py`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.1.0/txtfrompdf/extract.py` & `txt-from-pdf-1.1.1/txtfrompdf/extract.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import traceback
+from typing import Union
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from io import BytesIO
 
 from pdfminer.converter import TextConverter
 from pdfminer.layout import LAParams
 from pdfminer.pdfinterp import PDFPageInterpreter, PDFResourceManager
 from pdfminer.pdfpage import PDFPage
@@ -67,33 +68,36 @@
                 )
 
                 raise exc
 
     return pages
 
 
-def pdf_to_text(path):
+def pdf_to_text(path: Union[str, BytesIO]) -> str:
     manager = PDFResourceManager()
     retstr = BytesIO()
     layout = LAParams(all_texts=True)
     device = TextConverter(manager, retstr, laparams=layout)
-    filepath = open(path, "rb")
+    filepath = open(path, "rb") if isinstance(path, str) else path
     interpreter = PDFPageInterpreter(manager, device)
 
     try:
         for page in PDFPage.get_pages(filepath, check_extractable=False):
             interpreter.process_page(page)
 
     except (PDFSyntaxError, TypeError):
-        logger.error(f"ERROR: Extraction failed for {path}")
+        logger.error(f"ERROR: Extraction failed.")
 
     text = retstr.getvalue()
-    filepath.close()
     device.close()
     retstr.close()
+
+    if isinstance(path, str):
+        filepath.close()
+
     return text.decode("utf-8")  # decode from bytes to text
 
 
 def _extract_txt_from_pdf(pdf_file, split_into_pages=True, process_output=True):
 
     if not split_into_pages:
         text = pdf_to_text(pdf_file)
@@ -124,34 +128,44 @@
     # Post-process text
     if process_output:
         text = post_process(text, pdf_file)
 
     return text
 
 
-def extract_txt_from_pdf(pdf_file, split_into_pages=True, process_output=True):
+def extract_txt_from_pdf(pdf_file: Union[str, BytesIO], split_into_pages: bool = False, process_output: bool = True):
     """
     Extracts text from a PDF file and saves it to a text file.
 
     Args:
-        pdf_file (str): Path to the PDF file.
-        split_into_pages (bool, optional): Whether to split the PDF into individual pages during extraction or not. Defaults to True.
+        pdf_file (Union[str, BytesIO]): Path to the PDF file or a BytesIO object.
+        split_into_pages (bool, optional): Whether to split the PDF into individual pages during extraction or not. Defaults to False.
         process_output (bool, optional): Whether to post-process the extracted text. Defaults to True.
 
     Returns:
         str: Extracted text from the PDF file.
     """
+    if not isinstance(pdf_file, str) and split_into_pages:
+        # Binary inputs are not supported for splitting into pages
+        split_into_pages = False 
+        logger.warning("Binary inputs are not supported for splitting into pages. Setting split_into_pages=False. "
+                       "To suppress this warning, pass split_into_pages=False explicitly.")
+
+    if isinstance(pdf_file, bytes):
+        # Convert bytes to BytesIO object
+        pdf_file = BytesIO(pdf_file)
+
     try:
         text = _extract_txt_from_pdf(
             pdf_file, split_into_pages=split_into_pages, process_output=process_output
         )
         return text
     except PdfReadError:
         split_into_pages = not split_into_pages
-        logger.error(f"Retrying with split_into_pages={split_into_pages}")
+        logger.error(f"PDF Extraction failed! Retrying with split_into_pages={split_into_pages}")
         try:
             text = _extract_txt_from_pdf(
                 pdf_file,
                 split_into_pages=split_into_pages,
                 process_output=process_output,
             )
             return text
```

### Comparing `txt-from-pdf-1.1.0/txtfrompdf/filter.py` & `txt-from-pdf-1.1.1/txtfrompdf/filter.py`

 * *Files identical despite different names*

### Comparing `txt-from-pdf-1.1.0/txtfrompdf/fix_unicode.py` & `txt-from-pdf-1.1.1/txtfrompdf/fix_unicode.py`

 * *Files identical despite different names*

