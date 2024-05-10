# Comparing `tmp/utk_exodus-0.1.4.tar.gz` & `tmp/utk_exodus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.4.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.5.tar", max compression
```

## Comparing `utk_exodus-0.1.4.tar` & `utk_exodus-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2575 2024-05-08 21:11:48.505135 utk_exodus-0.1.4/README.md
--rw-r--r--   0        0        0      654 2024-05-09 12:54:40.198668 utk_exodus-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      440 2024-05-08 14:55:57.119783 utk_exodus-0.1.4/utk_exodus/__init__.py
--rw-r--r--   0        0        0     2387 2022-10-30 16:46:31.391736 utk_exodus-0.1.4/utk_exodus/config/samvera_default.yml
--rw-r--r--   0        0        0    12260 2024-05-06 16:36:47.872904 utk_exodus-0.1.4/utk_exodus/config/utk_dc.yml
--rw-r--r--   0        0        0    11044 2024-05-06 16:37:06.967592 utk_exodus-0.1.4/utk_exodus/config/utk_dc_no_uris.yml
--rw-r--r--   0        0        0     7824 2024-05-06 16:36:57.261544 utk_exodus-0.1.4/utk_exodus/config/utk_no_uris_no_names.yml
--rw-r--r--   0        0        0       43 2024-05-08 14:32:31.650721 utk_exodus-0.1.4/utk_exodus/controller/__init__.py
--rw-r--r--   0        0        0     4493 2024-05-09 12:53:43.841673 utk_exodus-0.1.4/utk_exodus/controller/controller.py
--rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.4/utk_exodus/curate/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.4/utk_exodus/curate/curate.py
--rw-r--r--   0        0        0     4049 2024-05-09 12:53:35.105919 utk_exodus-0.1.4/utk_exodus/exodus.py
--rw-r--r--   0        0        0       32 2024-05-08 12:26:21.007671 utk_exodus-0.1.4/utk_exodus/fedora/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-08 21:08:02.300387 utk_exodus-0.1.4/utk_exodus/fedora/fedora.py
--rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.4/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.4/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.4/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.4/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.4/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    39221 2024-05-08 23:29:50.024088 utk_exodus-0.1.4/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.4/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0     8833 2024-05-08 15:14:24.860576 utk_exodus-0.1.4/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.4/utk_exodus/validate/__init__.py
--rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.4/utk_exodus/validate/validate.py
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 utk_exodus-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3445 2024-05-09 14:09:03.042318 utk_exodus-0.1.5/README.md
+-rw-r--r--   0        0        0      654 2024-05-09 19:00:50.061735 utk_exodus-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      440 2024-05-08 14:55:57.119783 utk_exodus-0.1.5/utk_exodus/__init__.py
+-rw-r--r--   0        0        0     2387 2022-10-30 16:46:31.391736 utk_exodus-0.1.5/utk_exodus/config/samvera_default.yml
+-rw-r--r--   0        0        0    12260 2024-05-06 16:36:47.872904 utk_exodus-0.1.5/utk_exodus/config/utk_dc.yml
+-rw-r--r--   0        0        0    11044 2024-05-06 16:37:06.967592 utk_exodus-0.1.5/utk_exodus/config/utk_dc_no_uris.yml
+-rw-r--r--   0        0        0     7824 2024-05-06 16:36:57.261544 utk_exodus-0.1.5/utk_exodus/config/utk_no_uris_no_names.yml
+-rw-r--r--   0        0        0       43 2024-05-08 14:32:31.650721 utk_exodus-0.1.5/utk_exodus/controller/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-09 12:53:43.841673 utk_exodus-0.1.5/utk_exodus/controller/controller.py
+-rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.5/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.5/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     4049 2024-05-09 12:53:35.105919 utk_exodus-0.1.5/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       32 2024-05-08 12:26:21.007671 utk_exodus-0.1.5/utk_exodus/fedora/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-08 21:08:02.300387 utk_exodus-0.1.5/utk_exodus/fedora/fedora.py
+-rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.5/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.5/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.5/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.5/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.5/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    39241 2024-05-09 19:00:34.433616 utk_exodus-0.1.5/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.5/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0     8833 2024-05-08 15:14:24.860576 utk_exodus-0.1.5/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.5/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.5/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 utk_exodus-0.1.5/PKG-INFO
```

### Comparing `utk_exodus-0.1.4/README.md` & `utk_exodus-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,38 @@
 
 To install for use, ideally use `pipx`:
 
 ```shell
 pipx install utk_exodus
 ```
 
-The above will install the application in a virtual environment and make it available to you where ever you are in your
-path so you can use it from anywhere without needing to understand the intricacies of Python. 
+This will install the application in a virtual environment and make it available to you where ever you are in your
+path, so that you can use it from anywhere without needing to understand the intricacies of Python. 
 
 If you don't want to use `pipx`, you can install the whole library with the following command but do so mindfully:
 
 ```shell
 pip install utk_exodus
 ```
 
+## Before You Start
+
+Before you start, you need to have a few things in place:
+
+1. Exodus assumes you have the following environmental variables set appropriately:
+    * `FEDORA_USER`: this is a user with read access to the Fedora repository
+    * `FEDORA_PASSWORD`: the password for that Fedora user
+    * `FEDORA_URI`: the base URI for where Fedora is installed
+2. If you're looking for these values, you can find them in the Exodus `Environment` of this repository in `Settings`.
+
 ## Using
 
 There are several interfaces for the application.
 
-If you want to get works and files, and you have metadata files, use::
+If you want to get works and files, and you have metadata files, use:
 
 ```shell
 exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
 ```
 
 If you want to get works and files, and you don't have metadata files, you need to specify
 a collection and a work type:
@@ -48,21 +58,27 @@
 
 If for some reason you need to create a files sheet for  works after the fact, use:
 
 ```shell
 exodus add_files --sheet path/to/sheet.csv --files_sheet path/to/files_sheet.csv 
 ```
 
+## What's Missing Here Right Now
+
+* Appropriate application of restrictions
+* The ability to create pcdm:Collection objects.
+* The ability to create a new metadata import from a previous import
 
 ## Understanding Configs
 
-Exodus uses `yml` files for migration.  By default, exodus treats everything agnostically and relies on the `xpaths` 
-section of the base mapping to determine how a concept is mapped. If a property (or properties) have complex rules, a 
-class can be written to handle the special case.  When this happens, the `yml` should have a `special` property, and 
-it should be defined in `MetadataMapping().__lookup_special_property()`.
+Exodus migrates works and filesets according to [the UTK Metadata mapping](https://utk-mods-to-rdf.readthedocs.io/en/latest/contents/5_technical_metadata_properties.html#mapping).
+To do this, Exodus uses `yml` files for migration.  By default, exodus treats everything agnostically and relies on the 
+`xpaths` section of the base mapping to determine how a concept is mapped. If a property (or properties) have complex 
+rules, a class can be written to handle the special case.  When this happens, the `yml` should have a `special` 
+property, and it should be defined in `MetadataMapping().__lookup_special_property()`.
 
 An agnostic property should look like this in the `yml`:
 
 ```yml
   - name: table_of_contents
     xpaths:
       - 'mods:tableOfContents'
```

### Comparing `utk_exodus-0.1.4/pyproject.toml` & `utk_exodus-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utk-exodus"
-version = "0.1.4"
+version = "0.1.5"
 description = "A tool for building import sheets from UTK legacy systems"
 authors = ["Mark Baggett <mbagget1@utk.edu>"]
 readme = "README.md"
 include = [
     { path = "utk_exodus/config", format = ["sdist", "wheel"] }
 ]
```

### Comparing `utk_exodus-0.1.4/utk_exodus/config/samvera_default.yml` & `utk_exodus-0.1.5/utk_exodus/config/samvera_default.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/config/utk_dc.yml` & `utk_exodus-0.1.5/utk_exodus/config/utk_dc.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/config/utk_dc_no_uris.yml` & `utk_exodus-0.1.5/utk_exodus/config/utk_dc_no_uris.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/config/utk_no_uris_no_names.yml` & `utk_exodus-0.1.5/utk_exodus/config/utk_no_uris_no_names.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/controller/controller.py` & `utk_exodus-0.1.5/utk_exodus/controller/controller.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/curate/curate.py` & `utk_exodus-0.1.5/utk_exodus/curate/curate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/exodus.py` & `utk_exodus-0.1.5/utk_exodus/exodus.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/fedora/fedora.py` & `utk_exodus-0.1.5/utk_exodus/fedora/fedora.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/finder/finder.py` & `utk_exodus-0.1.5/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/metadata/__init__.py` & `utk_exodus-0.1.5/utk_exodus/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.5/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.5/utk_exodus/metadata/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -949,14 +949,15 @@
     def __find_unique_fieldnames(self, data):
         for k, v in data.items():
             if k not in self.fieldnames:
                 self.fieldnames.append(k)
         return
 
     def __dereference_islandora_type(self, file):
+        print(file)
         islandora_types = {
             "info:fedora/islandora:sp-audioCModel": "Audio",
             "info:fedora/islandora:bookCModel": "Book",
             "info:fedora/islandora:binaryObjectCModel": "Generic",
             "info:fedora/islandora:sp_large_image_cmodel": "Image",
             "info:fedora/islandora:sp_basic_image": "Image",
             "info:fedora/islandora:sp_pdf": "Pdf",
```

### Comparing `utk_exodus-0.1.4/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.5/utk_exodus/risearch/risearch.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.4/utk_exodus/validate/validate.py` & `utk_exodus-0.1.5/utk_exodus/validate/validate.py`

 * *Files identical despite different names*

