# Comparing `tmp/malariagen_data-9.0.0.tar.gz` & `tmp/malariagen_data-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malariagen_data-9.0.0.tar", max compression
+gzip compressed data, was "malariagen_data-9.0.1.tar", max compression
```

## Comparing `malariagen_data-9.0.0.tar` & `malariagen_data-9.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1067 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/LICENSE
--rw-r--r--   0        0        0     2954 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/README.md
--rw-r--r--   0        0        0      987 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/__init__.py
--rw-r--r--   0        0        0     7663 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/af1.py
--rw-r--r--   0        0        0    11997 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/ag3.py
--rw-r--r--   0        0        0     9451 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/amin1.py
--rw-r--r--   0        0        0        0 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/__init__.py
--rw-r--r--   0        0        0    10685 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/aim_data.py
--rw-r--r--   0        0        0      724 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/aim_params.py
--rw-r--r--   0        0        0    18834 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/base.py
--rw-r--r--   0        0        0     7078 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/base_params.py
--rw-r--r--   0        0        0    33307 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/cnv_data.py
--rw-r--r--   0        0        0      537 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/cnv_params.py
--rw-r--r--   0        0        0      903 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dash_params.py
--rw-r--r--   0        0        0    10036 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dipclust.py
--rw-r--r--   0        0        0      692 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/dipclust_params.py
--rw-r--r--   0        0        0      270 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/diplotype_distance_params.py
--rw-r--r--   0        0        0     2024 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/frq_params.py
--rw-r--r--   0        0        0    18115 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/fst.py
--rw-r--r--   0        0        0      690 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/fst_params.py
--rw-r--r--   0        0        0    21540 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/g123.py
--rw-r--r--   0        0        0     1083 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/g123_params.py
--rw-r--r--   0        0        0    15770 2024-04-26 06:46:31.144221 malariagen_data-9.0.0/malariagen_data/anoph/genome_features.py
--rw-r--r--   0        0        0     4300 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/genome_sequence.py
--rw-r--r--   0        0        0     2556 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/gplt_params.py
--rw-r--r--   0        0        0    16647 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h12.py
--rw-r--r--   0        0        0      739 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h12_params.py
--rw-r--r--   0        0        0    12730 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/h1x.py
--rw-r--r--   0        0        0    15233 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hap_data.py
--rw-r--r--   0        0        0      288 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hap_params.py
--rw-r--r--   0        0        0     9863 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapclust.py
--rw-r--r--   0        0        0      468 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapclust_params.py
--rw-r--r--   0        0        0      667 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/hapnet_params.py
--rw-r--r--   0        0        0     1323 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/het_params.py
--rw-r--r--   0        0        0     5883 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/igv.py
--rw-r--r--   0        0        0     2758 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/ihs_params.py
--rw-r--r--   0        0        0     1521 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/map_params.py
--rw-r--r--   0        0        0    15204 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/pca.py
--rw-r--r--   0        0        0      524 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/pca_params.py
--rw-r--r--   0        0        0     4533 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/plotly_params.py
--rw-r--r--   0        0        0    40182 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/sample_metadata.py
--rw-r--r--   0        0        0    64953 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/snp_data.py
--rw-r--r--   0        0        0    48792 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/snp_frq.py
--rw-r--r--   0        0        0      554 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/tree_params.py
--rw-r--r--   0        0        0     2046 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anoph/xpehh_params.py
--rw-r--r--   0        0        0   126711 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/anopheles.py
--rw-r--r--   0        0        0    10514 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/mjn.py
--rw-r--r--   0        0        0     1253 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pf7.py
--rw-r--r--   0        0        0     4442 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pf7_config.json
--rw-r--r--   0        0        0    11756 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/plasmodium.py
--rw-r--r--   0        0        0     3353 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/plotly_dendrogram.py
--rw-r--r--   0        0        0     1253 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pv4.py
--rw-r--r--   0        0        0     2060 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/pv4_config.json
--rw-r--r--   0        0        0    39556 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/util.py
--rw-r--r--   0        0        0    18170 2024-04-26 06:46:31.148221 malariagen_data-9.0.0/malariagen_data/veff.py
--rw-r--r--   0        0        0     2486 2024-04-26 06:46:49.708326 malariagen_data-9.0.0/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 malariagen_data-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/LICENSE
+-rw-r--r--   0        0        0     2954 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/README.md
+-rw-r--r--   0        0        0      987 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/__init__.py
+-rw-r--r--   0        0        0     7663 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/af1.py
+-rw-r--r--   0        0        0    11997 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/ag3.py
+-rw-r--r--   0        0        0     9451 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/amin1.py
+-rw-r--r--   0        0        0        0 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/__init__.py
+-rw-r--r--   0        0        0    10685 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/aim_data.py
+-rw-r--r--   0        0        0      724 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/aim_params.py
+-rw-r--r--   0        0        0    18834 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/base.py
+-rw-r--r--   0        0        0     7078 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/base_params.py
+-rw-r--r--   0        0        0    33307 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/cnv_data.py
+-rw-r--r--   0        0        0      537 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/cnv_params.py
+-rw-r--r--   0        0        0      903 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/dash_params.py
+-rw-r--r--   0        0        0    10036 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/dipclust.py
+-rw-r--r--   0        0        0      692 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/dipclust_params.py
+-rw-r--r--   0        0        0      270 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/diplotype_distance_params.py
+-rw-r--r--   0        0        0     2024 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/frq_params.py
+-rw-r--r--   0        0        0    18115 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/fst.py
+-rw-r--r--   0        0        0      690 2024-05-10 09:42:35.967680 malariagen_data-9.0.1/malariagen_data/anoph/fst_params.py
+-rw-r--r--   0        0        0    21540 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/g123.py
+-rw-r--r--   0        0        0     1083 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/g123_params.py
+-rw-r--r--   0        0        0    15770 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/genome_features.py
+-rw-r--r--   0        0        0     4300 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/genome_sequence.py
+-rw-r--r--   0        0        0     2556 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/gplt_params.py
+-rw-r--r--   0        0        0    16647 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/h12.py
+-rw-r--r--   0        0        0      739 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/h12_params.py
+-rw-r--r--   0        0        0    12730 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/h1x.py
+-rw-r--r--   0        0        0    15233 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/hap_data.py
+-rw-r--r--   0        0        0      288 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/hap_params.py
+-rw-r--r--   0        0        0     9863 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/hapclust.py
+-rw-r--r--   0        0        0      468 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/hapclust_params.py
+-rw-r--r--   0        0        0      667 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/hapnet_params.py
+-rw-r--r--   0        0        0     1323 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/het_params.py
+-rw-r--r--   0        0        0     5883 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/igv.py
+-rw-r--r--   0        0        0     2758 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/ihs_params.py
+-rw-r--r--   0        0        0     1521 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/map_params.py
+-rw-r--r--   0        0        0    15204 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/pca.py
+-rw-r--r--   0        0        0      524 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/pca_params.py
+-rw-r--r--   0        0        0     4533 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/plotly_params.py
+-rw-r--r--   0        0        0    40182 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/sample_metadata.py
+-rw-r--r--   0        0        0    64953 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/snp_data.py
+-rw-r--r--   0        0        0    48792 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/snp_frq.py
+-rw-r--r--   0        0        0      554 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/tree_params.py
+-rw-r--r--   0        0        0     2046 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anoph/xpehh_params.py
+-rw-r--r--   0        0        0   126711 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/anopheles.py
+-rw-r--r--   0        0        0    10514 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/mjn.py
+-rw-r--r--   0        0        0     1253 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/pf7.py
+-rw-r--r--   0        0        0     4442 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/pf7_config.json
+-rw-r--r--   0        0        0    11756 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/plasmodium.py
+-rw-r--r--   0        0        0     3353 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/plotly_dendrogram.py
+-rw-r--r--   0        0        0     1253 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/pv4.py
+-rw-r--r--   0        0        0     2060 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/pv4_config.json
+-rw-r--r--   0        0        0    39556 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/util.py
+-rw-r--r--   0        0        0    18170 2024-05-10 09:42:35.971680 malariagen_data-9.0.1/malariagen_data/veff.py
+-rw-r--r--   0        0        0     2486 2024-05-10 09:42:49.263700 malariagen_data-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 malariagen_data-9.0.1/PKG-INFO
```

### Comparing `malariagen_data-9.0.0/LICENSE` & `malariagen_data-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/README.md` & `malariagen_data-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/__init__.py` & `malariagen_data-9.0.1/malariagen_data/__init__.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/af1.py` & `malariagen_data-9.0.1/malariagen_data/af1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/ag3.py` & `malariagen_data-9.0.1/malariagen_data/ag3.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/amin1.py` & `malariagen_data-9.0.1/malariagen_data/amin1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/aim_data.py` & `malariagen_data-9.0.1/malariagen_data/anoph/aim_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/aim_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/aim_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/base.py` & `malariagen_data-9.0.1/malariagen_data/anoph/base.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/base_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/base_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/cnv_data.py` & `malariagen_data-9.0.1/malariagen_data/anoph/cnv_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/cnv_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/cnv_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/dash_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/dash_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/dipclust.py` & `malariagen_data-9.0.1/malariagen_data/anoph/dipclust.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/dipclust_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/dipclust_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/frq_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/frq_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/fst.py` & `malariagen_data-9.0.1/malariagen_data/anoph/fst.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/fst_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/fst_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/g123.py` & `malariagen_data-9.0.1/malariagen_data/anoph/g123.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/g123_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/g123_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/genome_features.py` & `malariagen_data-9.0.1/malariagen_data/anoph/genome_features.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/genome_sequence.py` & `malariagen_data-9.0.1/malariagen_data/anoph/genome_sequence.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/gplt_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/gplt_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/h12.py` & `malariagen_data-9.0.1/malariagen_data/anoph/h12.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/h12_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/h12_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/h1x.py` & `malariagen_data-9.0.1/malariagen_data/anoph/h1x.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/hap_data.py` & `malariagen_data-9.0.1/malariagen_data/anoph/hap_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/hapclust.py` & `malariagen_data-9.0.1/malariagen_data/anoph/hapclust.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/hapnet_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/hapnet_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/het_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/het_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/igv.py` & `malariagen_data-9.0.1/malariagen_data/anoph/igv.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/ihs_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/ihs_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/map_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/map_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/pca.py` & `malariagen_data-9.0.1/malariagen_data/anoph/pca.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/pca_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/pca_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/plotly_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/plotly_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/sample_metadata.py` & `malariagen_data-9.0.1/malariagen_data/anoph/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/snp_data.py` & `malariagen_data-9.0.1/malariagen_data/anoph/snp_data.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/snp_frq.py` & `malariagen_data-9.0.1/malariagen_data/anoph/snp_frq.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/tree_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/tree_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anoph/xpehh_params.py` & `malariagen_data-9.0.1/malariagen_data/anoph/xpehh_params.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/anopheles.py` & `malariagen_data-9.0.1/malariagen_data/anopheles.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/mjn.py` & `malariagen_data-9.0.1/malariagen_data/mjn.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/pf7.py` & `malariagen_data-9.0.1/malariagen_data/pf7.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/pf7_config.json` & `malariagen_data-9.0.1/malariagen_data/pf7_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/plasmodium.py` & `malariagen_data-9.0.1/malariagen_data/plasmodium.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/plotly_dendrogram.py` & `malariagen_data-9.0.1/malariagen_data/plotly_dendrogram.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/pv4.py` & `malariagen_data-9.0.1/malariagen_data/pv4.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/pv4_config.json` & `malariagen_data-9.0.1/malariagen_data/pv4_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/util.py` & `malariagen_data-9.0.1/malariagen_data/util.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/malariagen_data/veff.py` & `malariagen_data-9.0.1/malariagen_data/veff.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-9.0.0/pyproject.toml` & `malariagen_data-9.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "malariagen_data"
-version = "9.0.0"
+version = "9.0.1"
 description = "A package for accessing and analysing MalariaGEN data."
 readme = "README.md"
 documentation = "https://malariagen.github.io/malariagen-data-python/latest/"
 repository = "https://github.com/malariagen/malariagen-data-python"
 authors = [
     "Alistair Miles <alistair.miles@sanger.ac.uk>",
     "Chris Clarkson <cc28@sanger.ac.uk>",
```

### Comparing `malariagen_data-9.0.0/PKG-INFO` & `malariagen_data-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malariagen_data
-Version: 9.0.0
+Version: 9.0.1
 Summary: A package for accessing and analysing MalariaGEN data.
 Home-page: https://github.com/malariagen/malariagen-data-python
 License: MIT
 Author: Alistair Miles
 Author-email: alistair.miles@sanger.ac.uk
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

