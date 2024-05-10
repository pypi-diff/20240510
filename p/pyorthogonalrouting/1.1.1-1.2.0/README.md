# Comparing `tmp/pyorthogonalrouting-1.1.1.tar.gz` & `tmp/pyorthogonalrouting-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorthogonalrouting-1.1.1.tar", last modified: Thu May  2 17:17:23 2024, max compression
+gzip compressed data, was "pyorthogonalrouting-1.2.0.tar", last modified: Fri May 10 17:55:54 2024, max compression
```

## Comparing `pyorthogonalrouting-1.1.1.tar` & `pyorthogonalrouting-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821650 pyorthogonalrouting-1.1.1/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-06 14:22:10.000000 pyorthogonalrouting-1.1.1/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-02 17:17:23.821460 pyorthogonalrouting-1.1.1/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1811 2024-04-25 14:31:09.000000 pyorthogonalrouting-1.1.1/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      817 2024-04-29 00:18:49.000000 pyorthogonalrouting-1.1.1/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-02 17:17:23.821691 pyorthogonalrouting-1.1.1/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.813644 pyorthogonalrouting-1.1.1/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.819620 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      607 2024-04-11 13:00:44.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2545 2024-05-01 18:51:12.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Configuration.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      648 2024-04-10 14:41:49.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/ConnectorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4004 2024-04-08 00:38:06.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Functions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6405 2024-04-10 15:08:08.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Grid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      247 2024-04-04 20:00:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/LeftTopRightBottom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      390 2024-03-31 20:46:11.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Line.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6353 2024-04-13 14:41:34.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnector.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1039 2024-03-31 20:47:20.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2024-04-29 00:35:04.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      589 2024-04-07 17:06:45.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Point.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11420 2024-04-12 20:46:55.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointGraph.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2340 2024-04-11 20:33:20.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1036 2024-04-30 00:38:15.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rect.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5423 2024-04-08 20:44:33.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rectangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      424 2024-04-29 01:42:33.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Size.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       53 2024-04-06 14:24:59.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-01 18:57:25.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821128 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2024-03-31 20:53:59.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/BendDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      134 2024-04-01 17:04:50.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/Direction.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      154 2024-04-02 23:01:12.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/Side.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-31 19:08:00.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821274 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       21 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-10 17:55:54.316470 pyorthogonalrouting-1.2.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-06 14:22:10.000000 pyorthogonalrouting-1.2.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-10 17:55:54.316278 pyorthogonalrouting-1.2.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1811 2024-04-25 14:31:09.000000 pyorthogonalrouting-1.2.0/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      817 2024-04-29 00:18:49.000000 pyorthogonalrouting-1.2.0/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-10 17:55:54.316508 pyorthogonalrouting-1.2.0/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-10 17:55:54.306798 pyorthogonalrouting-1.2.0/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-10 17:55:54.314421 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      607 2024-04-11 13:00:44.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3845 2024-05-10 17:54:50.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Configuration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      648 2024-04-10 14:41:49.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/ConnectorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4004 2024-04-08 00:38:06.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Functions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6405 2024-04-10 15:08:08.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Grid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      247 2024-04-04 20:00:23.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/LeftTopRightBottom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      390 2024-03-31 20:46:11.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Line.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6353 2024-04-13 14:41:34.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnector.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1039 2024-03-31 20:47:20.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2024-04-29 00:35:04.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnectorOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      589 2024-04-07 17:06:45.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Point.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11420 2024-04-12 20:46:55.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/PointGraph.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2340 2024-04-11 20:33:20.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/PointNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1036 2024-04-30 00:38:15.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Rect.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5423 2024-04-08 20:44:33.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Rectangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      424 2024-04-29 01:42:33.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Size.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       53 2024-04-06 14:24:59.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-10 13:45:09.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-10 17:55:54.315941 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2024-03-31 20:53:59.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/BendDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      134 2024-04-01 17:04:50.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/Direction.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      154 2024-04-02 23:01:12.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/Side.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-31 19:08:00.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/enumerations/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-10 17:55:54.316077 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-10 17:55:54.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-05-10 17:55:54.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-10 17:55:54.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       21 2024-05-10 17:55:54.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2024-05-10 17:55:54.000000 pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/top_level.txt
```

### Comparing `pyorthogonalrouting-1.1.1/LICENSE` & `pyorthogonalrouting-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/PKG-INFO` & `pyorthogonalrouting-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorthogonalrouting
-Version: 1.1.1
+Version: 1.2.0
 Summary: Yet another orthogonal router
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/py-orthogonal-routing
 Keywords: orthogonal,routing,python,pyut
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.1.1 Summary: Yet
+Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.2.0 Summary: Yet
 another orthogonal router Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/py-orthogonal-routing Keywords:
 orthogonal,routing,python,pyut Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: codeallybasic==1.3.1 ![](https://github.com/
 hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-
```

### Comparing `pyorthogonalrouting-1.1.1/README.md` & `pyorthogonalrouting-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/pyproject.toml` & `pyorthogonalrouting-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Common.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Common.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/ConnectorPoint.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/ConnectorPoint.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Functions.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Functions.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Grid.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Grid.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnector.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnector.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorOptions.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/OrthogonalConnectorOptions.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Point.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Point.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointGraph.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/PointGraph.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointNode.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/PointNode.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rect.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Rect.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rectangle.py` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting/Rectangle.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/PKG-INFO` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorthogonalrouting
-Version: 1.1.1
+Version: 1.2.0
 Summary: Yet another orthogonal router
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/py-orthogonal-routing
 Keywords: orthogonal,routing,python,pyut
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.1.1 Summary: Yet
+Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.2.0 Summary: Yet
 another orthogonal router Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/py-orthogonal-routing Keywords:
 orthogonal,routing,python,pyut Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: codeallybasic==1.3.1 ![](https://github.com/
 hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-
```

### Comparing `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/SOURCES.txt` & `pyorthogonalrouting-1.2.0/src/pyorthogonalrouting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

