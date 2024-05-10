# Comparing `tmp/dbis_relational_model-1.0.1.tar.gz` & `tmp/dbis_relational_model-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis_relational_model-1.0.1.tar", last modified: Wed Apr 17 08:19:29 2024, max compression
+gzip compressed data, was "dbis_relational_model-1.0.2.tar", last modified: Fri May 10 13:45:05 2024, max compression
```

## Comparing `dbis_relational_model-1.0.1.tar` & `dbis_relational_model-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      903 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-17 08:00:00.000000 dbis_relational_model-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.414484 dbis_relational_model-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.414484 dbis_relational_model-1.0.1/src/dbis_relational_model/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-17 08:00:00.000000 dbis_relational_model-1.0.1/src/dbis_relational_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18225 2024-04-17 08:02:44.000000 dbis_relational_model-1.0.1/src/dbis_relational_model/relational_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      903 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 08:19:29.000000 dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:19:29.418484 dbis_relational_model-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4352 2024-04-17 08:02:44.000000 dbis_relational_model-1.0.1/tests/test_Task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:45:05.460367 dbis_relational_model-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      903 2024-05-10 13:45:05.460367 dbis_relational_model-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-02-06 11:28:22.000000 dbis_relational_model-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-10 13:29:27.000000 dbis_relational_model-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 13:45:05.460367 dbis_relational_model-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:45:05.456367 dbis_relational_model-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:45:05.456367 dbis_relational_model-1.0.2/src/dbis_relational_model/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-17 08:00:00.000000 dbis_relational_model-1.0.2/src/dbis_relational_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18891 2024-05-10 13:29:27.000000 dbis_relational_model-1.0.2/src/dbis_relational_model/relational_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:45:05.460367 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      903 2024-05-10 13:45:05.000000 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-10 13:45:05.000000 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 13:45:05.000000 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-10 13:45:05.000000 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-10 13:45:05.000000 dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:45:05.460367 dbis_relational_model-1.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2024-04-17 08:02:44.000000 dbis_relational_model-1.0.2/tests/test_Task.py
```

### Comparing `dbis_relational_model-1.0.1/LICENSE` & `dbis_relational_model-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis_relational_model-1.0.1/PKG-INFO` & `dbis_relational_model-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-model
-Version: 1.0.1
+Version: 1.0.2
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-relational-model
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis_relational_model-1.0.1/pyproject.toml` & `dbis_relational_model-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="dbis-relational-model"
-version='1.0.1'
+version='1.0.2'
 description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `dbis_relational_model-1.0.1/src/dbis_relational_model/relational_model.py` & `dbis_relational_model-1.0.2/src/dbis_relational_model/relational_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,26 +201,30 @@
 
             if curr_best is None:
                 penalty = scores["wrong_subset"] + scores["wrong_attribute"] * (
                     len(s1.rhs.attributes) + len(s1.lhs.attributes)
                 )
                 score += penalty
                 if debug:
+                    left = s1.lhs.relationName if s1.lhs is not None else "EMPTY"
+                    right = s1.rhs.relationName if s1.rhs is not None else "EMPTY"
                     print(
-                        f"Fehlende Untermengen-Abh. links={s1.lhs.relationName}, rechts={s1.rhs.relationName}: ziehe {penalty} Punkte ab"
+                        f"Fehlende Untermengen-Abh. links={left}, rechts={right}: ziehe {penalty} Punkte ab"
                     )
             else:
                 if debug:
                     # if missingLhs > 0:
                     #    print(f"Wrong attributes on left side: {missingLhs}")
                     # if missingRhs > 0:
                     #    print(f"Wrong attributes on right side: {missingRhs}")
+                    left = s1.lhs.relationName if s1.lhs is not None else "EMPTY"
+                    right = s1.rhs.relationName if s1.rhs is not None else "EMPTY"
                     if curr_best_score > 0:
                         print(
-                            f"Falsche Attribute in Untermengen-Abh. links={s1.lhs.relationName}, rechts={s1.rhs.relationName}: ziehe {curr_best_score} Punkte ab"
+                            f"Falsche Attribute in Untermengen-Abh. links={left}, rechts={right}: ziehe {curr_best_score} Punkte ab"
                         )
                 score += curr_best_score
 
         return score, relation_mappings
 
     def compare_intersections(
         self, rm, relation_mappings, scores, debug=False, label_threshold=0.8
@@ -305,26 +309,33 @@
 
             if curr_best is None:
                 penalty = scores["wrong_intersection"] + scores["wrong_attribute"] * (
                     len(i1.rhs.attributes) + len(i1.lhs.attributes)
                 )
                 score += penalty
                 if debug:
+                    left = i1.lhs.relationName if i1.lhs is not None else "EMPTY"
+                    right = i1.rhs.relationName if i1.rhs is not None else "EMPTY"
+                    equals = (
+                        i1.equals.relationName if i1.equals is not None else "EMPTY"
+                    )
                     print(
-                        f"Fehlender Schnitt: links={i1.lhs.relationName}, rechts={i1.rhs.relationName}, Schnittmenge={i1.equals.relationName}. Ziehe {penalty} Punkte ab"
+                        f"Fehlender Schnitt: links={left}, rechts={right}, Schnittmenge={equals}. Ziehe {penalty} Punkte ab"
                     )
             else:
                 if debug:
                     # if missingLhs > 0:
                     #    print(f"Wrong attributes on left side: {missingLhs}")
                     # if missingRhs > 0:
                     #    print(f"Wrong attributes on right side: {missingRhs}")
+                    left = i1.lhs.relationName if i1.lhs is not None else "EMPTY"
+                    right = i1.rhs.relationName if i1.rhs is not None else "EMPTY"
                     if curr_best_score > 0:
                         print(
-                            f"Falsche Attribute in Schnitt: linkeRelation={i1.lhs.relationName}, rechteRelation={i1.rhs.relationName}: ziehe {curr_best_score} Punkte ab"
+                            f"Falsche Attribute in Schnitt: linkeRelation={left}, rechteRelation={right}: ziehe {curr_best_score} Punkte ab"
                         )
                 score += curr_best_score
 
         return score, relation_mappings
 
     def compare_against(self, rm, scores, debug=False, label_threshold=0.8):
         if debug:
```

### Comparing `dbis_relational_model-1.0.1/src/dbis_relational_model.egg-info/PKG-INFO` & `dbis_relational_model-1.0.2/src/dbis_relational_model.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-model
-Version: 1.0.1
+Version: 1.0.2
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-relational-model
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis_relational_model-1.0.1/tests/test_Task.py` & `dbis_relational_model-1.0.2/tests/test_Task.py`

 * *Files identical despite different names*

