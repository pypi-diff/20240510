# Comparing `tmp/dumbo_asp-0.3.6.tar.gz` & `tmp/dumbo_asp-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_asp-0.3.6.tar", max compression
+gzip compressed data, was "dumbo_asp-0.3.7.tar", max compression
```

## Comparing `dumbo_asp-0.3.6.tar` & `dumbo_asp-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-01-09 17:04:55.577097 dumbo_asp-0.3.6/LICENSE
--rw-r--r--   0        0        0        0 2023-01-09 17:12:18.538163 dumbo_asp-0.3.6/dumbo_asp/__init__.py
--rw-r--r--   0        0        0        0 2023-09-30 10:54:04.086162 dumbo_asp-0.3.6/dumbo_asp/primitives/__init__.py
--rw-r--r--   0        0        0     5599 2024-02-22 07:47:30.762229 dumbo_asp-0.3.6/dumbo_asp/primitives/atoms.py
--rw-r--r--   0        0        0     9361 2024-03-09 20:07:14.220635 dumbo_asp-0.3.6/dumbo_asp/primitives/models.py
--rw-r--r--   0        0        0     3855 2024-02-18 09:48:10.547119 dumbo_asp-0.3.6/dumbo_asp/primitives/parsers.py
--rw-r--r--   0        0        0     2704 2024-02-22 17:17:34.892439 dumbo_asp-0.3.6/dumbo_asp/primitives/predicates.py
--rw-r--r--   0        0        0     9512 2024-03-09 20:06:20.660565 dumbo_asp-0.3.6/dumbo_asp/primitives/programs.py
--rw-r--r--   0        0        0    23255 2024-03-05 14:32:35.582972 dumbo_asp-0.3.6/dumbo_asp/primitives/rules.py
--rw-r--r--   0        0        0     9498 2023-11-27 14:09:14.732245 dumbo_asp-0.3.6/dumbo_asp/primitives/templates.py
--rw-r--r--   0        0        0     4117 2023-09-30 10:39:16.827298 dumbo_asp-0.3.6/dumbo_asp/primitives/terms.py
--rw-r--r--   0        0        0    30755 2024-03-09 20:06:20.660565 dumbo_asp-0.3.6/dumbo_asp/queries.py
--rw-r--r--   0        0        0      722 2023-11-27 15:51:35.759497 dumbo_asp-0.3.6/dumbo_asp/templates/binary_relations.template.asp
--rw-r--r--   0        0        0      480 2023-11-27 14:08:46.682144 dumbo_asp-0.3.6/dumbo_asp/templates/dumbo.template.asp
--rw-r--r--   0        0        0     1639 2023-11-27 14:11:09.232886 dumbo_asp-0.3.6/dumbo_asp/templates/graphs.template.asp
--rw-r--r--   0        0        0     1516 2023-11-27 15:20:52.662693 dumbo_asp-0.3.6/dumbo_asp/templates/sets.template.asp
--rw-r--r--   0        0        0     1718 2023-09-14 13:12:54.715666 dumbo_asp-0.3.6/dumbo_asp/utils.py
--rw-r--r--   0        0        0      525 2024-03-09 20:07:29.608655 dumbo_asp-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 dumbo_asp-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-09 17:04:55.577097 dumbo_asp-0.3.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-09 17:12:18.538163 dumbo_asp-0.3.7/dumbo_asp/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-30 10:54:04.086162 dumbo_asp-0.3.7/dumbo_asp/primitives/__init__.py
+-rw-r--r--   0        0        0     5599 2024-02-22 07:47:30.762229 dumbo_asp-0.3.7/dumbo_asp/primitives/atoms.py
+-rw-r--r--   0        0        0     9361 2024-03-09 20:07:14.220635 dumbo_asp-0.3.7/dumbo_asp/primitives/models.py
+-rw-r--r--   0        0        0     3855 2024-02-18 09:48:10.547119 dumbo_asp-0.3.7/dumbo_asp/primitives/parsers.py
+-rw-r--r--   0        0        0     2704 2024-02-22 17:17:34.892439 dumbo_asp-0.3.7/dumbo_asp/primitives/predicates.py
+-rw-r--r--   0        0        0     9512 2024-03-09 20:06:20.660565 dumbo_asp-0.3.7/dumbo_asp/primitives/programs.py
+-rw-r--r--   0        0        0    23255 2024-03-05 14:32:35.582972 dumbo_asp-0.3.7/dumbo_asp/primitives/rules.py
+-rw-r--r--   0        0        0     9498 2023-11-27 14:09:14.732245 dumbo_asp-0.3.7/dumbo_asp/primitives/templates.py
+-rw-r--r--   0        0        0     4117 2023-09-30 10:39:16.827298 dumbo_asp-0.3.7/dumbo_asp/primitives/terms.py
+-rw-r--r--   0        0        0    30755 2024-03-14 16:54:42.435108 dumbo_asp-0.3.7/dumbo_asp/queries.py
+-rw-r--r--   0        0        0      722 2023-11-27 15:51:35.759497 dumbo_asp-0.3.7/dumbo_asp/templates/binary_relations.template.asp
+-rw-r--r--   0        0        0      480 2023-11-27 14:08:46.682144 dumbo_asp-0.3.7/dumbo_asp/templates/dumbo.template.asp
+-rw-r--r--   0        0        0     1639 2023-11-27 14:11:09.232886 dumbo_asp-0.3.7/dumbo_asp/templates/graphs.template.asp
+-rw-r--r--   0        0        0     1516 2023-11-27 15:20:52.662693 dumbo_asp-0.3.7/dumbo_asp/templates/sets.template.asp
+-rw-r--r--   0        0        0     1718 2023-09-14 13:12:54.715666 dumbo_asp-0.3.7/dumbo_asp/utils.py
+-rw-r--r--   0        0        0      581 2024-05-10 15:48:46.711432 dumbo_asp-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 dumbo_asp-0.3.7/PKG-INFO
```

### Comparing `dumbo_asp-0.3.6/LICENSE` & `dumbo_asp-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/atoms.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/atoms.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/models.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/models.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/parsers.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/parsers.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/predicates.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/predicates.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/programs.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/programs.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/rules.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/rules.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/templates.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/templates.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/primitives/terms.py` & `dumbo_asp-0.3.7/dumbo_asp/primitives/terms.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/queries.py` & `dumbo_asp-0.3.7/dumbo_asp/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,16 +477,16 @@
     """
     Compute an explanation graph for a conjunctive query.
     :param program: The program of interest (including facts, possibly partially expanded and reordered)
     :param answer_set: All true atoms from the program (the program must not have #show directives)
     :param herbrand_base: Some atoms of interest in addition to those mentioned in the answer set and in the query
     :param query: The conjunctive query in the form of facts (truth values implicit from the answer set)
     :param collect_pus_program: An optional list that will be extended with four programs:
-    [0] the symbolic program used to compute the 1-PUS;
-    [1] the selectors in the program (in the form of facts);
+    [0] the selectors in the program (in the form of facts);
+    [1] the symbolic program used to compute the 1-PUS;
     [2] the reduced selectors being the preferred 1-PUS;
     [3] the expanded program (at index 0) including the preferred 1-PUS (at index 2).
     :return: a graph encoded by predicates node and link (with labels on nodes and links)
     """
     pus_program = __explanation_graph_pus_program(program, answer_set, herbrand_base, query,
                                                   collect_pus_program=collect_pus_program)
```

### Comparing `dumbo_asp-0.3.6/dumbo_asp/templates/binary_relations.template.asp` & `dumbo_asp-0.3.7/dumbo_asp/templates/binary_relations.template.asp`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/templates/graphs.template.asp` & `dumbo_asp-0.3.7/dumbo_asp/templates/graphs.template.asp`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/templates/sets.template.asp` & `dumbo_asp-0.3.7/dumbo_asp/templates/sets.template.asp`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/dumbo_asp/utils.py` & `dumbo_asp-0.3.7/dumbo_asp/utils.py`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.3.6/PKG-INFO` & `dumbo_asp-0.3.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dumbo-asp
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities for Answer Set Programming
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Pillow (>=10.2.0,<11.0.0)
-Requires-Dist: cairocffi (>=1.6.0,<2.0.0)
+Requires-Dist: Pillow (>=10.3.0,<11.0.0)
+Requires-Dist: cairocffi (>=1.7.0,<2.0.0)
 Requires-Dist: clingo (>=5.7.1,<6.0.0)
-Requires-Dist: clingox (>=1.2.0,<2.0.0)
+Requires-Dist: clingox (>=1.2.1,<2.0.0)
 Requires-Dist: dateutils (>=0.6.12,<0.7.0)
-Requires-Dist: distlib (>=0.3.7,<0.4.0)
-Requires-Dist: dumbo-utils (>=0.3.1,<0.4.0)
-Requires-Dist: igraph (>=0.11.3,<0.12.0)
+Requires-Dist: distlib (>=0.3.8,<0.4.0)
+Requires-Dist: dumbo-utils (>=0.3.2,<0.4.0)
+Requires-Dist: igraph (>=0.11.5,<0.12.0)
```

