# Comparing `tmp/chemopy2-1.0.4.tar.gz` & `tmp/chemopy2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemopy2-1.0.4.tar", last modified: Fri Nov 17 08:13:48 2023, max compression
+gzip compressed data, was "chemopy2-1.0.5.tar", last modified: Fri May 10 20:49:46 2024, max compression
```

## Comparing `chemopy2-1.0.4.tar` & `chemopy2-1.0.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.237882 chemopy2-1.0.4/
--rw-rw-rw-   0        0        0    35821 2023-07-05 07:45:47.000000 chemopy2-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      482 2023-07-13 07:36:12.000000 chemopy2-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1973 2023-11-17 08:13:48.236882 chemopy2-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5913 2023-07-13 07:55:08.000000 chemopy2-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.169360 chemopy2-1.0.4/docs/
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.179468 chemopy2-1.0.4/docs/source/
--rw-rw-rw-   0        0        0     4414 2023-07-11 06:44:19.000000 chemopy2-1.0.4/docs/source/chemopy.rst
--rw-rw-rw-   0        0        0    10658 2023-07-11 06:48:27.000000 chemopy2-1.0.4/docs/source/conf.py
--rw-rw-rw-   0        0        0      491 2023-07-11 06:43:29.000000 chemopy2-1.0.4/docs/source/index.rst
--rw-rw-rw-   0        0        0       64 2023-07-11 06:48:27.000000 chemopy2-1.0.4/docs/source/modules.rst
--rw-rw-rw-   0        0        0     2640 2023-11-17 08:13:48.243881 chemopy2-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      155 2023-07-13 08:32:08.000000 chemopy2-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.170982 chemopy2-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.206261 chemopy2-1.0.4/src/chemopy/
--rw-rw-rw-   0        0        0      307 2023-11-17 08:13:25.000000 chemopy2-1.0.4/src/chemopy/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-07-13 08:28:35.000000 chemopy2-1.0.4/src/chemopy/asa.py
--rw-rw-rw-   0        0        0     9305 2023-07-13 08:28:35.000000 chemopy2-1.0.4/src/chemopy/atomproperty.py
--rw-rw-rw-   0        0        0     4990 2023-07-10 14:23:03.000000 chemopy2-1.0.4/src/chemopy/atomtypes.py
--rw-rw-rw-   0        0        0    10698 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/basak.py
--rw-rw-rw-   0        0        0     6041 2023-07-13 08:29:21.000000 chemopy2-1.0.4/src/chemopy/bcut.py
--rw-rw-rw-   0        0        0    12504 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/charge.py
--rw-rw-rw-   0        0        0     8423 2023-10-05 11:45:19.000000 chemopy2-1.0.4/src/chemopy/chemopy.py
--rw-rw-rw-   0        0        0    18860 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/connectivity.py
--rw-rw-rw-   0        0        0     9636 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/constitution.py
--rw-rw-rw-   0        0        0    11349 2023-07-13 08:29:29.000000 chemopy2-1.0.4/src/chemopy/cpsa.py
--rw-rw-rw-   0        0        0   248861 2023-07-13 07:07:32.000000 chemopy2-1.0.4/src/chemopy/descs.json
--rw-rw-rw-   0        0        0     8776 2023-07-13 08:29:29.000000 chemopy2-1.0.4/src/chemopy/estate.py
--rw-rw-rw-   0        0        0     7676 2023-10-13 09:28:44.000000 chemopy2-1.0.4/src/chemopy/fingerprint.py
--rw-rw-rw-   0        0        0     3538 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/fingerprint3d.py
--rw-rw-rw-   0        0        0     3836 2023-07-13 08:29:40.000000 chemopy2-1.0.4/src/chemopy/geary.py
--rw-rw-rw-   0        0        0    17084 2023-07-13 08:21:06.000000 chemopy2-1.0.4/src/chemopy/geo_opt.py
--rw-rw-rw-   0        0        0    18660 2023-07-13 08:29:58.000000 chemopy2-1.0.4/src/chemopy/geometric.py
--rw-rw-rw-   0        0        0     3914 2023-07-13 07:51:51.000000 chemopy2-1.0.4/src/chemopy/getmol.py
--rw-rw-rw-   0        0        0     5320 2023-07-13 08:29:58.000000 chemopy2-1.0.4/src/chemopy/kappa.py
--rw-rw-rw-   0        0        0     4152 2023-07-13 08:30:03.000000 chemopy2-1.0.4/src/chemopy/moe.py
--rw-rw-rw-   0        0        0     3930 2023-08-14 12:36:21.000000 chemopy2-1.0.4/src/chemopy/molproperty.py
--rw-rw-rw-   0        0        0     3615 2023-07-13 08:30:13.000000 chemopy2-1.0.4/src/chemopy/moran.py
--rw-rw-rw-   0        0        0     3317 2023-07-13 08:30:19.000000 chemopy2-1.0.4/src/chemopy/moreaubroto.py
--rw-rw-rw-   0        0        0    10626 2023-07-13 08:30:23.000000 chemopy2-1.0.4/src/chemopy/morse.py
--rw-rw-rw-   0        0        0     7203 2023-07-13 08:30:28.000000 chemopy2-1.0.4/src/chemopy/quanchem.py
--rw-rw-rw-   0        0        0      469 2023-07-05 07:45:47.000000 chemopy2-1.0.4/src/chemopy/radius.py
--rw-rw-rw-   0        0        0     7992 2023-07-13 08:30:41.000000 chemopy2-1.0.4/src/chemopy/rdf.py
--rw-rw-rw-   0        0        0    19631 2023-11-17 07:34:44.000000 chemopy2-1.0.4/src/chemopy/topology.py
--rw-rw-rw-   0        0        0     8477 2023-07-11 13:17:10.000000 chemopy2-1.0.4/src/chemopy/utils.py
--rw-rw-rw-   0        0        0    13776 2023-07-11 10:53:28.000000 chemopy2-1.0.4/src/chemopy/vector3d.py
--rw-rw-rw-   0        0        0    19997 2023-07-13 08:30:55.000000 chemopy2-1.0.4/src/chemopy/whim.py
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.220807 chemopy2-1.0.4/src/chemopy2.egg-info/
--rw-rw-rw-   0        0        0     1973 2023-11-17 08:13:48.000000 chemopy2-1.0.4/src/chemopy2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2023-11-17 08:13:48.000000 chemopy2-1.0.4/src/chemopy2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 08:13:48.000000 chemopy2-1.0.4/src/chemopy2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 07:52:13.000000 chemopy2-1.0.4/src/chemopy2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      184 2023-11-17 08:13:48.000000 chemopy2-1.0.4/src/chemopy2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-17 08:13:48.000000 chemopy2-1.0.4/src/chemopy2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.226798 chemopy2-1.0.4/tests/
--rw-rw-rw-   0        0        0       58 2023-07-10 20:00:28.000000 chemopy2-1.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-07-12 16:55:35.000000 chemopy2-1.0.4/tests/constants.py
-drwxrwxrwx   0        0        0        0 2023-11-17 08:13:48.235894 chemopy2-1.0.4/tests/samples/
--rw-rw-rw-   0        0        0    10635 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/CID148124.mol
--rw-rw-rw-   0        0        0    11654 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/CID148124.mol2
--rw-rw-rw-   0        0        0       45 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/cas.txt
--rw-rw-rw-   0        0        0     2055 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/drug.mol
--rw-rw-rw-   0        0        0       43 2023-07-12 17:19:32.000000 chemopy2-1.0.4/tests/samples/drugbank.txt
--rw-rw-rw-   0        0        0      571 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/drugs.inchi
--rw-rw-rw-   0        0        0    33996 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/drugs.sdf
--rw-rw-rw-   0        0        0      259 2023-07-12 17:18:35.000000 chemopy2-1.0.4/tests/samples/ebi.txt
--rw-rw-rw-   0        0        0       40 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/kegg.txt
--rw-rw-rw-   0        0        0       28 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/ncbi.txt
--rw-rw-rw-   0        0        0     1291 2023-07-05 07:45:47.000000 chemopy2-1.0.4/tests/samples/testmol.smi
--rw-rw-rw-   0        0        0     3874 2023-07-13 06:40:56.000000 chemopy2-1.0.4/tests/test_descs_fps.py
--rw-rw-rw-   0        0        0     1406 2023-07-13 07:21:50.000000 chemopy2-1.0.4/tests/test_details.py
--rw-rw-rw-   0        0        0     1320 2023-07-12 16:55:39.000000 chemopy2-1.0.4/tests/test_fetchmols.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.992242 chemopy2-1.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-07-05 07:45:47.000000 chemopy2-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      482 2023-07-13 07:36:12.000000 chemopy2-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1973 2024-05-10 20:49:46.992242 chemopy2-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5913 2023-07-13 07:55:08.000000 chemopy2-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.642419 chemopy2-1.0.5/docs/
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.694083 chemopy2-1.0.5/docs/source/
+-rw-rw-rw-   0        0        0     4414 2023-07-11 06:44:19.000000 chemopy2-1.0.5/docs/source/chemopy.rst
+-rw-rw-rw-   0        0        0    10658 2023-07-11 06:48:27.000000 chemopy2-1.0.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      491 2023-07-11 06:43:29.000000 chemopy2-1.0.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0       64 2023-07-11 06:48:27.000000 chemopy2-1.0.5/docs/source/modules.rst
+-rw-rw-rw-   0        0        0     2640 2024-05-10 20:49:46.992242 chemopy2-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      155 2023-07-13 08:32:08.000000 chemopy2-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.642419 chemopy2-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.882425 chemopy2-1.0.5/src/chemopy/
+-rw-rw-rw-   0        0        0      307 2024-05-10 20:49:14.000000 chemopy2-1.0.5/src/chemopy/__init__.py
+-rw-rw-rw-   0        0        0     3735 2023-07-13 08:28:35.000000 chemopy2-1.0.5/src/chemopy/asa.py
+-rw-rw-rw-   0        0        0     9305 2023-07-13 08:28:35.000000 chemopy2-1.0.5/src/chemopy/atomproperty.py
+-rw-rw-rw-   0        0        0     4990 2023-07-10 14:23:03.000000 chemopy2-1.0.5/src/chemopy/atomtypes.py
+-rw-rw-rw-   0        0        0    10698 2023-08-14 12:36:21.000000 chemopy2-1.0.5/src/chemopy/basak.py
+-rw-rw-rw-   0        0        0     6041 2023-07-13 08:29:21.000000 chemopy2-1.0.5/src/chemopy/bcut.py
+-rw-rw-rw-   0        0        0    12504 2023-08-14 12:36:21.000000 chemopy2-1.0.5/src/chemopy/charge.py
+-rw-rw-rw-   0        0        0     8423 2023-10-05 11:45:19.000000 chemopy2-1.0.5/src/chemopy/chemopy.py
+-rw-rw-rw-   0        0        0    18836 2024-05-10 20:45:10.000000 chemopy2-1.0.5/src/chemopy/connectivity.py
+-rw-rw-rw-   0        0        0     9636 2023-08-14 12:36:21.000000 chemopy2-1.0.5/src/chemopy/constitution.py
+-rw-rw-rw-   0        0        0    11349 2023-07-13 08:29:29.000000 chemopy2-1.0.5/src/chemopy/cpsa.py
+-rw-rw-rw-   0        0        0   248861 2023-07-13 07:07:32.000000 chemopy2-1.0.5/src/chemopy/descs.json
+-rw-rw-rw-   0        0        0     8776 2023-07-13 08:29:29.000000 chemopy2-1.0.5/src/chemopy/estate.py
+-rw-rw-rw-   0        0        0     7676 2023-10-13 09:28:44.000000 chemopy2-1.0.5/src/chemopy/fingerprint.py
+-rw-rw-rw-   0        0        0     3538 2023-08-14 12:36:21.000000 chemopy2-1.0.5/src/chemopy/fingerprint3d.py
+-rw-rw-rw-   0        0        0     3836 2023-07-13 08:29:40.000000 chemopy2-1.0.5/src/chemopy/geary.py
+-rw-rw-rw-   0        0        0    17084 2023-07-13 08:21:06.000000 chemopy2-1.0.5/src/chemopy/geo_opt.py
+-rw-rw-rw-   0        0        0    18660 2023-07-13 08:29:58.000000 chemopy2-1.0.5/src/chemopy/geometric.py
+-rw-rw-rw-   0        0        0     3914 2023-07-13 07:51:51.000000 chemopy2-1.0.5/src/chemopy/getmol.py
+-rw-rw-rw-   0        0        0     5320 2023-07-13 08:29:58.000000 chemopy2-1.0.5/src/chemopy/kappa.py
+-rw-rw-rw-   0        0        0     4152 2023-07-13 08:30:03.000000 chemopy2-1.0.5/src/chemopy/moe.py
+-rw-rw-rw-   0        0        0     3930 2023-08-14 12:36:21.000000 chemopy2-1.0.5/src/chemopy/molproperty.py
+-rw-rw-rw-   0        0        0     3615 2023-07-13 08:30:13.000000 chemopy2-1.0.5/src/chemopy/moran.py
+-rw-rw-rw-   0        0        0     3317 2023-07-13 08:30:19.000000 chemopy2-1.0.5/src/chemopy/moreaubroto.py
+-rw-rw-rw-   0        0        0    10626 2023-07-13 08:30:23.000000 chemopy2-1.0.5/src/chemopy/morse.py
+-rw-rw-rw-   0        0        0     7203 2023-07-13 08:30:28.000000 chemopy2-1.0.5/src/chemopy/quanchem.py
+-rw-rw-rw-   0        0        0      469 2023-07-05 07:45:47.000000 chemopy2-1.0.5/src/chemopy/radius.py
+-rw-rw-rw-   0        0        0     7992 2023-07-13 08:30:41.000000 chemopy2-1.0.5/src/chemopy/rdf.py
+-rw-rw-rw-   0        0        0    19791 2024-05-10 20:45:03.000000 chemopy2-1.0.5/src/chemopy/topology.py
+-rw-rw-rw-   0        0        0     8477 2023-07-11 13:17:10.000000 chemopy2-1.0.5/src/chemopy/utils.py
+-rw-rw-rw-   0        0        0    13776 2023-07-11 10:53:28.000000 chemopy2-1.0.5/src/chemopy/vector3d.py
+-rw-rw-rw-   0        0        0    19997 2023-07-13 08:30:55.000000 chemopy2-1.0.5/src/chemopy/whim.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.976619 chemopy2-1.0.5/src/chemopy2.egg-info/
+-rw-rw-rw-   0        0        0     1973 2024-05-10 20:49:46.000000 chemopy2-1.0.5/src/chemopy2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-05-10 20:49:46.000000 chemopy2-1.0.5/src/chemopy2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 20:49:46.000000 chemopy2-1.0.5/src/chemopy2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 07:52:13.000000 chemopy2-1.0.5/src/chemopy2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      184 2024-05-10 20:49:46.000000 chemopy2-1.0.5/src/chemopy2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 20:49:46.000000 chemopy2-1.0.5/src/chemopy2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.929310 chemopy2-1.0.5/tests/
+-rw-rw-rw-   0        0        0       58 2023-07-10 20:00:28.000000 chemopy2-1.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-07-12 16:55:35.000000 chemopy2-1.0.5/tests/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:49:46.976619 chemopy2-1.0.5/tests/samples/
+-rw-rw-rw-   0        0        0    10635 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/CID148124.mol
+-rw-rw-rw-   0        0        0    11654 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/CID148124.mol2
+-rw-rw-rw-   0        0        0       45 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/cas.txt
+-rw-rw-rw-   0        0        0     2055 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/drug.mol
+-rw-rw-rw-   0        0        0       43 2023-07-12 17:19:32.000000 chemopy2-1.0.5/tests/samples/drugbank.txt
+-rw-rw-rw-   0        0        0      571 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/drugs.inchi
+-rw-rw-rw-   0        0        0    33996 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/drugs.sdf
+-rw-rw-rw-   0        0        0      259 2023-07-12 17:18:35.000000 chemopy2-1.0.5/tests/samples/ebi.txt
+-rw-rw-rw-   0        0        0       40 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/kegg.txt
+-rw-rw-rw-   0        0        0       28 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/ncbi.txt
+-rw-rw-rw-   0        0        0     1291 2023-07-05 07:45:47.000000 chemopy2-1.0.5/tests/samples/testmol.smi
+-rw-rw-rw-   0        0        0     3874 2023-07-13 06:40:56.000000 chemopy2-1.0.5/tests/test_descs_fps.py
+-rw-rw-rw-   0        0        0     1406 2023-07-13 07:21:50.000000 chemopy2-1.0.5/tests/test_details.py
+-rw-rw-rw-   0        0        0     1320 2023-07-12 16:55:39.000000 chemopy2-1.0.5/tests/test_fetchmols.py
```

### Comparing `chemopy2-1.0.4/LICENSE` & `chemopy2-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/PKG-INFO` & `chemopy2-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemopy2
-Version: 1.0.4
+Version: 1.0.5
 Summary: "A Python library calculating molecular descriptors."
 Home-page: https://github.com/OlivierBeq/chemopy
 Download-URL: https://github.com/OlivierBeq/chemopy/releases
 Author: "Dongsheng Cao, Yizeng Liang"
 Author-email: "oriental-cds@163.com"
 Maintainer: "Olivier J. M. Béquignon"
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
```

### Comparing `chemopy2-1.0.4/README.md` & `chemopy2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/docs/source/chemopy.rst` & `chemopy2-1.0.5/docs/source/chemopy.rst`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/docs/source/conf.py` & `chemopy2-1.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/setup.cfg` & `chemopy2-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/asa.py` & `chemopy2-1.0.5/src/chemopy/asa.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/atomproperty.py` & `chemopy2-1.0.5/src/chemopy/atomproperty.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/atomtypes.py` & `chemopy2-1.0.5/src/chemopy/atomtypes.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/basak.py` & `chemopy2-1.0.5/src/chemopy/basak.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/bcut.py` & `chemopy2-1.0.5/src/chemopy/bcut.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/charge.py` & `chemopy2-1.0.5/src/chemopy/charge.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/chemopy.py` & `chemopy2-1.0.5/src/chemopy/chemopy.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/connectivity.py` & `chemopy2-1.0.5/src/chemopy/connectivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 class Connectivity:
     """Topological indices"""
 
     @staticmethod
     def calculate_chi0(mol: Chem.Mol) -> float:
         """Calculate molecular connectivity chi index for path order 0."""
         deltas = [x.GetDegree() for x in mol.GetAtoms()]
-        while [0] in deltas:
-            deltas.remove([0])
         deltas = np.array(deltas, 'd')
+        deltas = deltas[deltas != 0]
         res = sum(np.sqrt(1. / deltas))
         return res
 
     @staticmethod
     def calculate_chi1(mol: Chem.Mol) -> float:
         """Calculate molecular connectivity chi index for path order 1."""
         cc = [x.GetBeginAtom().GetDegree() * x.GetEndAtom().GetDegree() for x in mol.GetBonds()]
```

### Comparing `chemopy2-1.0.4/src/chemopy/constitution.py` & `chemopy2-1.0.5/src/chemopy/constitution.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/cpsa.py` & `chemopy2-1.0.5/src/chemopy/cpsa.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/descs.json` & `chemopy2-1.0.5/src/chemopy/descs.json`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/estate.py` & `chemopy2-1.0.5/src/chemopy/estate.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/fingerprint.py` & `chemopy2-1.0.5/src/chemopy/fingerprint.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/fingerprint3d.py` & `chemopy2-1.0.5/src/chemopy/fingerprint3d.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/geary.py` & `chemopy2-1.0.5/src/chemopy/geary.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/geo_opt.py` & `chemopy2-1.0.5/src/chemopy/geo_opt.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/geometric.py` & `chemopy2-1.0.5/src/chemopy/geometric.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/getmol.py` & `chemopy2-1.0.5/src/chemopy/getmol.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/kappa.py` & `chemopy2-1.0.5/src/chemopy/kappa.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/moe.py` & `chemopy2-1.0.5/src/chemopy/moe.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/molproperty.py` & `chemopy2-1.0.5/src/chemopy/molproperty.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/moran.py` & `chemopy2-1.0.5/src/chemopy/moran.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/moreaubroto.py` & `chemopy2-1.0.5/src/chemopy/moreaubroto.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/morse.py` & `chemopy2-1.0.5/src/chemopy/morse.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/quanchem.py` & `chemopy2-1.0.5/src/chemopy/quanchem.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/rdf.py` & `chemopy2-1.0.5/src/chemopy/rdf.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/topology.py` & `chemopy2-1.0.5/src/chemopy/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,22 @@
         else:
             J = 0
         return J
 
     @staticmethod
     def calculate_graph_distance(mol: Chem.Mol) -> float:
         """Get graph distance index.
-    
+
         Or Tigdi.
         """
         Distance = Chem.GetDistanceMatrix(mol)
-        n = int(Distance.max())
         res = 0.0
-        for i in range(n):
-            temp = 1. / 2 * sum(sum(Distance == i + 1))
+        for i in np.unique(Distance.ravel()):
+            if i == 0 or i == 1.e+08: continue
+            temp = 1. / 2 * sum(sum(Distance == i))
             res = res + temp ** 2
         return np.log10(res)
 
     @staticmethod
     def calculate_diameter(mol: Chem.Mol) -> float:
         """Get largest value of the distance matrix.
     
@@ -384,44 +384,46 @@
         """Get total information index on distance equality.
     
         Or DET.
         """
         Distance = Chem.GetDistanceMatrix(mol)
         nAT = mol.GetNumAtoms()
         n = 1. / 2 * nAT ** 2 - nAT
-        DisType = int(Distance.max())
         res = 0.0
-        for i in range(DisType):
-            cc = 1. / 2 * sum(sum(Distance == i + 1))
-            res += cc * np.log2(cc)
+        for i in np.unique(Distance.ravel()):
+            if i == 1.e+08: continue
+            cc = 1. / 2 * sum(sum(Distance == i))
+            if cc > 0:
+                res += cc * np.log2(cc)
         return n * np.log2(n) - res if n > 0 else np.NaN
 
     @staticmethod
     def _calculate_entropy(Probability: Iterable[float]) -> float:
         """calculate_ entropy (Information content) of given probability."""
         res = 0.0
-        for i in Probability:
-            if i != 0:
-                res = res - i * np.log2(i)
+        Probability = np.array(Probability)
+        for i in Probability[Probability != 0]:
+            res = res - i * np.log2(i)
         return res
 
     @staticmethod
     def calculate_distance_equality_mean_inf(mol: Chem.Mol) -> float:
         """Get the mean information index on distance equality.
     
         Or IDE.
         """
         Distance = Chem.GetDistanceMatrix(mol)
         nAT = mol.GetNumAtoms()
         n = 1. / 2 * nAT ** 2 - nAT
         DisType = int(Distance.max())
         res = 0.0
         cc = np.zeros(DisType, dtype=float)
-        for i in range(DisType):
-            cc[i] = 1. / 2 * sum(sum(Distance == i + 1))
+        for i in np.unique(Distance.ravel()).astype(int):
+            if i == 1.e+08: continue
+            cc[i - 1] = 1. / 2 * sum(sum(Distance == i))
         res = Topology._calculate_entropy(cc / n)
         return res
 
     @staticmethod
     def calculate_vertex_equality_total_inf(mol: Chem.Mol) -> float:
         """Get the total information index on vertex equality.
```

### Comparing `chemopy2-1.0.4/src/chemopy/utils.py` & `chemopy2-1.0.5/src/chemopy/utils.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/vector3d.py` & `chemopy2-1.0.5/src/chemopy/vector3d.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy/whim.py` & `chemopy2-1.0.5/src/chemopy/whim.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/src/chemopy2.egg-info/PKG-INFO` & `chemopy2-1.0.5/src/chemopy2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemopy2
-Version: 1.0.4
+Version: 1.0.5
 Summary: "A Python library calculating molecular descriptors."
 Home-page: https://github.com/OlivierBeq/chemopy
 Download-URL: https://github.com/OlivierBeq/chemopy/releases
 Author: "Dongsheng Cao, Yizeng Liang"
 Author-email: "oriental-cds@163.com"
 Maintainer: "Olivier J. M. Béquignon"
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
```

### Comparing `chemopy2-1.0.4/src/chemopy2.egg-info/SOURCES.txt` & `chemopy2-1.0.5/src/chemopy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/constants.py` & `chemopy2-1.0.5/tests/constants.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/CID148124.mol` & `chemopy2-1.0.5/tests/samples/CID148124.mol`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/CID148124.mol2` & `chemopy2-1.0.5/tests/samples/CID148124.mol2`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/drug.mol` & `chemopy2-1.0.5/tests/samples/drug.mol`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/drugs.inchi` & `chemopy2-1.0.5/tests/samples/drugs.inchi`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/drugs.sdf` & `chemopy2-1.0.5/tests/samples/drugs.sdf`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/samples/testmol.smi` & `chemopy2-1.0.5/tests/samples/testmol.smi`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/test_descs_fps.py` & `chemopy2-1.0.5/tests/test_descs_fps.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/test_details.py` & `chemopy2-1.0.5/tests/test_details.py`

 * *Files identical despite different names*

### Comparing `chemopy2-1.0.4/tests/test_fetchmols.py` & `chemopy2-1.0.5/tests/test_fetchmols.py`

 * *Files identical despite different names*

