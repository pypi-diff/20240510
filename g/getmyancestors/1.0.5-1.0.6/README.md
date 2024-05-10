# Comparing `tmp/getmyancestors-1.0.5.tar.gz` & `tmp/getmyancestors-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmyancestors-1.0.5.tar", last modified: Tue Nov 21 17:19:24 2023, max compression
+gzip compressed data, was "getmyancestors-1.0.6.tar", last modified: Fri May 10 14:33:11 2024, max compression
```

## Comparing `getmyancestors-1.0.5.tar` & `getmyancestors-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bfontaine  (1000) bfontaine  (1000)        0 2023-11-21 17:19:24.435081 getmyancestors-1.0.5/
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      709 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/LICENSE
--rw-r--r--   0 bfontaine  (1000) bfontaine  (1000)     3301 2023-11-21 17:19:24.435081 getmyancestors-1.0.5/PKG-INFO
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     2630 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/README.md
-drwxrwxr-x   0 bfontaine  (1000) bfontaine  (1000)        0 2023-11-21 17:19:24.431081 getmyancestors-1.0.5/getmyancestors/
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      100 2023-11-21 17:01:01.000000 getmyancestors-1.0.5/getmyancestors/__init__.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)       65 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/getmyancestors/__main__.py
-drwxrwxr-x   0 bfontaine  (1000) bfontaine  (1000)        0 2023-11-21 17:19:24.435081 getmyancestors-1.0.5/getmyancestors/classes/
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)        0 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/getmyancestors/classes/__init__.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     1824 2023-11-21 16:59:23.000000 getmyancestors-1.0.5/getmyancestors/classes/constants.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)    12385 2023-11-21 16:58:29.000000 getmyancestors-1.0.5/getmyancestors/classes/gedcom.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)    24133 2023-11-21 16:59:20.000000 getmyancestors-1.0.5/getmyancestors/classes/gui.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     6505 2023-11-21 17:08:54.000000 getmyancestors-1.0.5/getmyancestors/classes/session.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     7326 2023-11-21 16:59:11.000000 getmyancestors-1.0.5/getmyancestors/classes/translation.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)    32658 2023-11-21 16:58:58.000000 getmyancestors-1.0.5/getmyancestors/classes/tree.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      198 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/getmyancestors/fstogedcom.png
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      546 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/getmyancestors/fstogedcom.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     8689 2023-11-21 16:58:29.000000 getmyancestors-1.0.5/getmyancestors/getmyancestors.py
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     4376 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/getmyancestors/mergemyancestors.py
-drwxrwxr-x   0 bfontaine  (1000) bfontaine  (1000)        0 2023-11-21 17:19:24.435081 getmyancestors-1.0.5/getmyancestors.egg-info/
--rw-r--r--   0 bfontaine  (1000) bfontaine  (1000)     3301 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/PKG-INFO
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      680 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/SOURCES.txt
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)        1 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/dependency_links.txt
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)      170 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/entry_points.txt
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)       73 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/requires.txt
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)       15 2023-11-21 17:19:24.000000 getmyancestors-1.0.5/getmyancestors.egg-info/top_level.txt
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)     1010 2023-11-20 08:51:30.000000 getmyancestors-1.0.5/pyproject.toml
--rw-rw-r--   0 bfontaine  (1000) bfontaine  (1000)       38 2023-11-21 17:19:24.435081 getmyancestors-1.0.5/setup.cfg
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2024-05-10 14:33:11.403682 getmyancestors-1.0.6/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      709 2023-01-21 19:10:46.000000 getmyancestors-1.0.6/LICENSE
+-rw-r--r--   0 benoit    (1000) benoit    (1000)     3301 2024-05-10 14:33:11.403682 getmyancestors-1.0.6/PKG-INFO
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     2630 2023-01-21 19:10:46.000000 getmyancestors-1.0.6/README.md
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2024-05-10 14:33:11.399682 getmyancestors-1.0.6/getmyancestors/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      100 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/__init__.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       65 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/__main__.py
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2024-05-10 14:33:11.403682 getmyancestors-1.0.6/getmyancestors/classes/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)        0 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/__init__.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     1824 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/constants.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    12493 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/gedcom.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    24133 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/gui.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     6505 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/session.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     7326 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/translation.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    32737 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/classes/tree.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      198 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/fstogedcom.png
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      546 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/fstogedcom.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     8689 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/getmyancestors.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     4441 2024-05-10 14:32:28.000000 getmyancestors-1.0.6/getmyancestors/mergemyancestors.py
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2024-05-10 14:33:11.403682 getmyancestors-1.0.6/getmyancestors.egg-info/
+-rw-r--r--   0 benoit    (1000) benoit    (1000)     3301 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      680 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)        1 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      170 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       73 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       15 2024-05-10 14:33:11.000000 getmyancestors-1.0.6/getmyancestors.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     1010 2023-08-27 12:48:05.000000 getmyancestors-1.0.6/pyproject.toml
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       38 2024-05-10 14:33:11.403682 getmyancestors-1.0.6/setup.cfg
```

### Comparing `getmyancestors-1.0.5/LICENSE` & `getmyancestors-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/PKG-INFO` & `getmyancestors-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getmyancestors
-Version: 1.0.5
+Version: 1.0.6
 Summary: Retrieve GEDCOM data from FamilySearch Tree
 License: GNU
 Project-URL: HomePage, https://github.com/Linekio/getmyancestors
 Keywords: getmyancestors,familysearch,fstogedcom,gedcom
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `getmyancestors-1.0.5/README.md` & `getmyancestors-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/constants.py` & `getmyancestors-1.0.6/getmyancestors/classes/constants.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/gedcom.py` & `getmyancestors-1.0.6/getmyancestors/classes/gedcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,16 @@
                 self.indi[self.num].gender = self.data
             elif self.tag in FACT_TYPES or self.tag == "EVEN":
                 self.indi[self.num].facts.add(self.__get_fact())
             elif self.tag == "BAPL":
                 self.indi[self.num].baptism = self.__get_ordinance()
             elif self.tag == "CONL":
                 self.indi[self.num].confirmation = self.__get_ordinance()
+            elif self.tag == "WAC":
+                self.indi[self.num].initiatory = self.__get_ordinance()
             elif self.tag == "ENDL":
                 self.indi[self.num].endowment = self.__get_ordinance()
             elif self.tag == "SLGC":
                 self.indi[self.num].sealing_child = self.__get_ordinance()
             elif self.tag == "FAMS":
                 self.indi[self.num].fams_num.add(int(self.data[2 : len(self.data) - 1]))
             elif self.tag == "FAMC":
```

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/gui.py` & `getmyancestors-1.0.6/getmyancestors/classes/gui.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/session.py` & `getmyancestors-1.0.6/getmyancestors/classes/session.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/translation.py` & `getmyancestors-1.0.6/getmyancestors/classes/translation.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/classes/tree.py` & `getmyancestors-1.0.6/getmyancestors/classes/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from getmyancestors.classes.constants import (
     MAX_PERSONS,
     FACT_EVEN,
     FACT_TAGS,
     ORDINANCES_STATUS,
 )
 
+
 # getmyancestors classes and functions
 def cont(string):
     """parse a GEDCOM line adding CONT and CONT tags if necessary"""
     level = int(string[:1]) + 1
     lines = string.splitlines()
     res = list()
     max_len = 255
@@ -363,16 +364,17 @@
                         )
                     for source in sources["sourceDescriptions"]:
                         if source["id"] not in self.tree.sources:
                             self.tree.sources[source["id"]] = Source(source, self.tree)
                         self.sources.add(
                             (self.tree.sources[source["id"]], quotes[source["id"]])
                         )
-            if "evidence" in data:
-                url = "/platform/tree/persons/%s/memories" % self.fid
+            for evidence in data.get("evidence", []):
+                memory_id, *_ = evidence["id"].partition("-")
+                url = "/platform/memories/memories/%s" % memory_id
                 memorie = self.tree.fs.get_url(url)
                 if memorie and "sourceDescriptions" in memorie:
                     for x in memorie["sourceDescriptions"]:
                         if x["mediaType"] == "text/plain":
                             text = "\n".join(
                                 val.get("value", "")
                                 for val in x.get("titles", [])
```

### Comparing `getmyancestors-1.0.5/getmyancestors/fstogedcom.py` & `getmyancestors-1.0.6/getmyancestors/fstogedcom.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/getmyancestors.py` & `getmyancestors-1.0.6/getmyancestors/getmyancestors.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/getmyancestors/mergemyancestors.py` & `getmyancestors-1.0.6/getmyancestors/mergemyancestors.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             tree.indi[fid].gender = ged.indi[num].gender
             tree.indi[fid].facts = ged.indi[num].facts
             tree.indi[fid].notes = ged.indi[num].notes
             tree.indi[fid].sources = ged.indi[num].sources
             tree.indi[fid].memories = ged.indi[num].memories
             tree.indi[fid].baptism = ged.indi[num].baptism
             tree.indi[fid].confirmation = ged.indi[num].confirmation
+            tree.indi[fid].initiatory = ged.indi[num].initiatory
             tree.indi[fid].endowment = ged.indi[num].endowment
             if not (tree.indi[fid].sealing_child and tree.indi[fid].sealing_child.famc):
                 tree.indi[fid].sealing_child = ged.indi[num].sealing_child
 
         # add information about families
         for num in ged.fam:
             husb, wife = (ged.fam[num].husb_fid, ged.fam[num].wife_fid)
```

### Comparing `getmyancestors-1.0.5/getmyancestors.egg-info/PKG-INFO` & `getmyancestors-1.0.6/getmyancestors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getmyancestors
-Version: 1.0.5
+Version: 1.0.6
 Summary: Retrieve GEDCOM data from FamilySearch Tree
 License: GNU
 Project-URL: HomePage, https://github.com/Linekio/getmyancestors
 Keywords: getmyancestors,familysearch,fstogedcom,gedcom
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `getmyancestors-1.0.5/getmyancestors.egg-info/SOURCES.txt` & `getmyancestors-1.0.6/getmyancestors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.5/pyproject.toml` & `getmyancestors-1.0.6/pyproject.toml`

 * *Files identical despite different names*

